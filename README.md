<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>南宁周末逃跑计划 🎀</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;800&display=swap');
        
        body {
            /* 使用可爱的圆润英文字体和系统中文字体 */
            font-family: 'Nunito', -apple-system, BlinkMacSystemFont, "PingFang SC", "Microsoft YaHei", sans-serif;
            /* 制作手账本的波点背景底纹 */
            background-color: #FFF5F7;
            background-image: radial-gradient(#FFD1DC 1.5px, transparent 1.5px);
            background-size: 24px 24px;
        }

        /* 自定义滚动条，使其更符合整体风格 */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #FFF5F7;
        }
        ::-webkit-scrollbar-thumb {
            background: #FFB6C1;
            border-radius: 10px;
        }
        
        /* 拍立得照片风格的阴影和边框 */
        .polaroid {
            background: white;
            padding: 8px 8px 24px 8px;
            box-shadow: 0 4px 6px -1px rgba(255, 182, 193, 0.3), 0 2px 4px -1px rgba(255, 182, 193, 0.2);
            transform: rotate(-2deg);
            transition: transform 0.3s ease;
        }
        .polaroid:hover {
            transform: rotate(1deg) scale(1.02);
            z-index: 10;
        }
        .polaroid-right {
            transform: rotate(3deg);
        }
        .polaroid-right:hover {
            transform: rotate(-1deg) scale(1.02);
        }

        /* 纸胶带效果 */
        .washi-tape {
            position: absolute;
            width: 90px;
            height: 28px;
            background-color: rgba(255, 182, 193, 0.6);
            top: -12px;
            left: 50%;
            transform: translateX(-50%) rotate(-3deg);
            z-index: 20;
            border-left: 2px dashed rgba(255,255,255,0.6);
            border-right: 2px dashed rgba(255,255,255,0.6);
            backdrop-filter: blur(2px);
        }
        .washi-tape.blue { background-color: rgba(167, 192, 253, 0.6); transform: translateX(-50%) rotate(2deg); }
        .washi-tape.yellow { background-color: rgba(253, 224, 71, 0.6); transform: translateX(-50%) rotate(-1deg); }

        /* 便利贴与复选框 */
        .sticky-note {
            background-color: #FEF9C3;
            box-shadow: 3px 4px 10px rgba(0,0,0,0.05);
            border-bottom-right-radius: 24px 6px;
        }
        .check-item { transition: all 0.2s ease; cursor: pointer; }
        .check-item.done { text-decoration: line-through; color: #a1a1aa; }
    </style>
</head>
<body class="min-h-screen text-gray-700 py-8 px-4 sm:px-8">

    <div class="max-w-2xl mx-auto">
        
        <!-- 头部区域：标题与简介 -->
        <header class="text-center mb-10 relative">
            <!-- 装饰性元素 -->
            <div class="absolute -top-6 -left-4 text-4xl animate-bounce" style="animation-duration: 3s;">✨</div>
            <div class="absolute top-10 -right-2 text-3xl animate-pulse">🌸</div>
            
            <div class="inline-block bg-white px-8 py-6 rounded-3xl shadow-sm border-2 border-pink-200 border-dashed relative">
                <div class="absolute -top-3 left-1/2 transform -translate-x-1/2 bg-pink-400 text-white text-xs font-bold px-3 py-1 rounded-full shadow-md tracking-wider">
                    WEEKEND ESCAPE
                </div>
                <h1 class="text-3xl sm:text-4xl font-extrabold text-pink-500 tracking-tight mb-2 mt-2">
                    🎀 南宁 48h 逃跑计划
                </h1>
                <h2 class="text-lg text-pink-400 font-medium mb-4">
                    小仙女的周末打卡日记 📝
                </h2>
                <p class="text-sm text-gray-500 leading-relaxed max-w-sm mx-auto">
                    周五下班就出发！逃离喧嚣，去山野里吸氧，去老街里嗦粉。一份完美涵盖吃住行的南宁出片攻略请查收~ 💕
                </p>
                
                <!-- 标签组 -->
                <div class="flex flex-wrap justify-center gap-2 mt-4 text-xs font-semibold">
                    <span class="bg-indigo-100 text-indigo-600 px-3 py-1.5 rounded-full"># 星夜出逃</span>
                    <span class="bg-pink-100 text-pink-600 px-3 py-1.5 rounded-full"># 绝美民宿</span>
                    <span class="bg-blue-100 text-blue-600 px-3 py-1.5 rounded-full"># 拍照绝绝子</span>
                </div>
            </div>
        </header>

        <!-- 行李备忘录 (便利贴风格) -->
        <section class="mb-12 flex justify-center">
            <div class="sticky-note relative p-6 w-full max-w-sm rounded-lg border border-yellow-200 transform rotate-1 hover:rotate-0 transition-transform">
                <div class="washi-tape yellow"></div>
                <h3 class="text-xl font-bold text-yellow-700 mb-4 text-center flex items-center justify-center gap-2">
                    <span>📋</span> 出发前清单
                </h3>
                <ul class="space-y-3 text-gray-700 font-medium">
                    <li class="check-item flex items-center gap-3" onclick="toggleCheck(this)">
                        <input type="checkbox" class="w-4 h-4 text-yellow-500 rounded border-yellow-400 focus:ring-yellow-500 pointer-events-none">
                        <span>身份证、学生证 (部分景点半价)</span>
                    </li>
                    <li class="check-item flex items-center gap-3" onclick="toggleCheck(this)">
                        <input type="checkbox" class="w-4 h-4 text-yellow-500 rounded border-yellow-400 focus:ring-yellow-500 pointer-events-none">
                        <span>充电宝、相机 (拍照必备📸)</span>
                    </li>
                    <li class="check-item flex items-center gap-3" onclick="toggleCheck(this)">
                        <input type="checkbox" class="w-4 h-4 text-yellow-500 rounded border-yellow-400 focus:ring-yellow-500 pointer-events-none">
                        <span>换洗仙女裙、舒适平底鞋</span>
                    </li>
                    <li class="check-item flex items-center gap-3" onclick="toggleCheck(this)">
                        <input type="checkbox" class="w-4 h-4 text-yellow-500 rounded border-yellow-400 focus:ring-yellow-500 pointer-events-none">
                        <span>肠胃药 (防嗦粉水土不服💊)</span>
                    </li>
                </ul>
                <p class="text-xs text-yellow-600 mt-5 text-center opacity-80">💡 点击文字即可划掉打卡哦！</p>
            </div>
        </section>

        <!-- DAY 0 模块 (周五晚) -->
        <section class="mb-12">
            <div class="flex items-center mb-6">
                <div class="bg-gradient-to-r from-indigo-400 to-indigo-300 text-white font-bold py-1 px-4 rounded-l-full rounded-r-full shadow-md flex items-center shadow-indigo-200">
                    <span class="text-xl mr-2">🌙</span>
                    <span>DAY 00 | 星夜出逃</span>
                </div>
                <div class="flex-grow border-t-2 border-indigo-200 border-dashed ml-4"></div>
            </div>

            <div class="relative pl-6 sm:pl-10 border-l-4 border-indigo-100 border-dotted space-y-8 ml-4">
                
                <!-- 行程 1 -->
                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-indigo-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🚄</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-indigo-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">19:30 快乐启程</h4>
                            <span class="text-xs font-bold text-indigo-500 bg-indigo-50 px-2 py-1 rounded-lg">逃离工位</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed mb-3">
                            周五下班直接冲向高铁站！带上精心准备的仙女裙，在车上敷个面膜，和姐妹一起期待美好的周末~ 目标：<strong>南宁东站</strong>！💨
                        </p>
                    </div>
                </div>

                <!-- 行程 2 -->
                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-indigo-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🏨</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-indigo-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">22:30 抵达仙女基地</h4>
                            <span class="text-xs font-bold text-blue-500 bg-blue-50 px-2 py-1 rounded-lg">奶油风民宿</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed">
                            入住提前订好的<strong>朝阳广场/青秀区</strong>附近的法式复古民宿（出行超方便！）。放下行李，在香香的浴缸里泡个澡洗去班味，美美地睡个美容觉，为明天的特种兵打卡充电！🛁✨
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- DAY 1 模块 -->
        <section class="mb-12">
            <div class="flex items-center mb-6">
                <div class="bg-gradient-to-r from-pink-400 to-pink-300 text-white font-bold py-1 px-4 rounded-l-full rounded-r-full shadow-md flex items-center shadow-pink-200">
                    <span class="text-xl mr-2">💖</span>
                    <span>DAY 01 | 老城与晚风</span>
                </div>
                <div class="flex-grow border-t-2 border-pink-200 border-dashed ml-4"></div>
            </div>

            <!-- 时间轴容器 -->
            <div class="relative pl-6 sm:pl-10 border-l-4 border-pink-100 border-dotted space-y-8 ml-4">
                
                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-pink-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🍜</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-pink-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">11:00 寻味老城</h4>
                            <span class="text-xs font-bold text-pink-400 bg-pink-50 px-2 py-1 rounded-lg">嗦粉达人</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed mb-3">
                            睡到自然醒！出门的第一站，当然是一碗酸辣开胃的<strong>老友粉</strong>啦！再配上一份酸甜爽脆的<strong>“酸嘢”</strong>，瞬间唤醒南方味蕾，简直不要太幸福~ 🤤
                        </p>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-pink-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">📸</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-pink-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">14:00 粗野自然</h4>
                            <span class="text-xs font-bold text-teal-500 bg-teal-50 px-2 py-1 rounded-lg">废土风出片</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed mb-4">
                            前往<strong>园博园·矿坑花园</strong>。谁能想到废弃采石场居然这么好拍！穿上酷酷的衣服或者仙女裙，下沉式极简美学让你分分钟拍出杂志大片。
                        </p>
                        <div class="w-48 mx-auto polaroid relative">
                            <div class="washi-tape"></div>
                            <img src="https://placehold.co/400x300/FFE4E1/FF69B4?text=Click!+📸" alt="矿坑花园" class="w-full h-auto rounded-sm">
                        </div>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-pink-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">✨</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-pink-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">17:00 历史质感</h4>
                            <span class="text-xs font-bold text-purple-400 bg-purple-50 px-2 py-1 rounded-lg">非遗美学</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed">
                            来<strong>区博物馆新馆</strong>吹吹空调。在极简光影中，近距离观赏苗银的Bling Bling和壮锦的精妙细节，感受沉淀下来的浪漫。
                        </p>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-pink-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🏮</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-pink-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">19:30 换装夜游</h4>
                            <span class="text-xs font-bold text-red-400 bg-red-50 px-2 py-1 rounded-lg">沉浸式体验</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed">
                            夜幕降临，去<strong>三街两巷</strong>。青砖黛瓦下，挑一套绝美的苗族/壮族服饰，化身苗疆少女，在灯笼下拍一组氛围感夜景写真！🎆
                        </p>
                    </div>
                </div>

            </div>
        </section>

        <!-- DAY 2 模块 -->
        <section class="mb-10">
            <div class="flex items-center mb-6">
                <div class="bg-gradient-to-r from-purple-400 to-purple-300 text-white font-bold py-1 px-4 rounded-l-full rounded-r-full shadow-md flex items-center shadow-purple-200">
                    <span class="text-xl mr-2">🌿</span>
                    <span>DAY 02 | 森林与咖啡</span>
                </div>
                <div class="flex-grow border-t-2 border-purple-200 border-dashed ml-4"></div>
            </div>

            <!-- 时间轴容器 -->
            <div class="relative pl-6 sm:pl-10 border-l-4 border-purple-100 border-dotted space-y-8 ml-4">
                
                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-purple-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🧚‍♀️</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-purple-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">09:30 绿野寻光</h4>
                            <span class="text-xs font-bold text-green-500 bg-green-50 px-2 py-1 rounded-lg">森系精灵</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed mb-4">
                            早起去<strong>青秀山·荫生植物园</strong>！穿梭在比人还高的巨大蕨类与绝美兰花中，捕捉清晨神仙般的丁达尔效应，当一日森林精灵。🌲
                        </p>
                        <div class="w-48 mx-auto polaroid polaroid-right relative">
                            <div class="washi-tape blue"></div>
                            <img src="https://placehold.co/400x300/E0F8E9/2E8B57?text=Forest+Vibes" alt="青秀山" class="w-full h-auto rounded-sm">
                        </div>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-purple-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🍧</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-purple-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">12:30 桂味新尝</h4>
                            <span class="text-xs font-bold text-orange-400 bg-orange-50 px-2 py-1 rounded-lg">干饭人</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed">
                            午餐安排！品尝外酥里嫩的<strong>巴马烤香猪</strong>和鲜美的<strong>老友鱼</strong>，体验新派桂菜精致又接地气的烟火气。
                        </p>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-purple-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">☕</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-purple-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">14:30 工业与咖啡</h4>
                            <span class="text-xs font-bold text-amber-500 bg-amber-50 px-2 py-1 rounded-lg">打卡圣地</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed">
                            下午茶时间~ 来到<strong>百益·上河城</strong>。在红砖老厂房改造的复古街区逛逛，点一杯广西特色的<strong>水牛奶拿铁</strong>，享受慢时光。
                        </p>
                    </div>
                </div>

                <div class="relative">
                    <div class="absolute -left-[38px] sm:-left-[54px] top-0 bg-white border-4 border-purple-100 text-xl rounded-full w-10 h-10 flex items-center justify-center shadow-sm">🚉</div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-purple-50 hover:shadow-md transition-shadow">
                        <div class="flex items-baseline justify-between mb-2">
                            <h4 class="font-bold text-lg text-gray-800">18:00 满载而归</h4>
                            <span class="text-xs font-bold text-rose-500 bg-rose-50 px-2 py-1 rounded-lg">下次见啦</span>
                        </div>
                        <p class="text-sm text-gray-600 leading-relaxed">
                            带着满手机的人生照片、吃得饱饱的肚子，坐上返程的高铁。结束完美的周末逃跑计划，南宁，我们下次再见啦！👋💕
                        </p>
                    </div>
                </div>

            </div>
        </section>

        <!-- 底部 -->
        <footer class="text-center mt-12 pb-8">
            <div class="inline-block bg-white/60 backdrop-blur-sm px-6 py-3 rounded-full border border-pink-100 shadow-sm text-sm font-medium text-pink-400">
                ⭐ 下周一也要做个元气打工人噢 ⭐
            </div>
            <div class="mt-4 text-xs text-gray-400 flex justify-center items-center space-x-1">
                <span>Made with</span>
                <span class="text-red-400 animate-pulse">❤</span>
                <span>for Nanning Escape</span>
            </div>
        </footer>

    </div>

    <script>
        function toggleCheck(element) {
            // 切换完成样式的 class
            element.classList.toggle('done');
            // 同步切换复选框的状态
            const checkbox = element.querySelector('input[type="checkbox"]');
            checkbox.checked = !checkbox.checked;
        }
    </script>
</body>
</html>
