<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الدليل الشامل للذكاء الاصطناعي - جوكر لينك</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(to bottom, #1a1a1a 0%, #2d2d2d 50%, #3d3d3d 100%);
            background-attachment: fixed;
            min-height: 100vh;
            padding: 20px;
            position: relative;
        }
        
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(ellipse at bottom, rgba(218, 165, 32, 0.3) 0%, transparent 60%);
            pointer-events: none;
            z-index: 0;
        }
        
        .container {
            position: relative;
            z-index: 1;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        /* Header */
        .header {
            text-align: center;
            color: white;
            margin-bottom: 40px;
            animation: fadeInDown 0.8s;
        }

        .header h1 {
            font-size: 3em;
            margin-bottom: 15px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .header p {
            font-size: 1.3em;
            margin-bottom: 20px;
        }

        .whatsapp-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1em;
            box-shadow: 0 4px 15px rgba(218, 165, 32, 0.4);
            transition: all 0.3s;
        }

        .whatsapp-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(218, 165, 32, 0.6);
            background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
        }

        /* Tabs */
        .tabs {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .tab-btn {
            background: rgba(255, 255, 255, 0.1);
            color: white;
            border: 2px solid rgba(218, 165, 32, 0.3);
            padding: 15px 30px;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 1em;
            backdrop-filter: blur(10px);
        }

        .tab-btn.active {
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
            border-color: #FFD700;
            box-shadow: 0 4px 15px rgba(218, 165, 32, 0.4);
        }

        .tab-btn:hover {
            transform: translateY(-2px);
            border-color: #DAA520;
        }

        /* Categories */
        .categories {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .category-btn {
            background: rgba(255, 255, 255, 0.1);
            color: white;
            border: 1px solid rgba(218, 165, 32, 0.3);
            padding: 10px 20px;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 0.9em;
            backdrop-filter: blur(10px);
        }

        .category-btn.active {
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
            border-color: #FFD700;
        }

        /* Apps Grid */
        .apps-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 25px;
            margin-bottom: 40px;
        }

        .app-card {
            background: rgba(30, 30, 30, 0.95);
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            transition: all 0.3s;
            animation: fadeInUp 0.6s;
            border: 1px solid rgba(218, 165, 32, 0.2);
        }

        .app-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(218, 165, 32, 0.3);
            border-color: rgba(218, 165, 32, 0.5);
        }

        .app-card.highlight {
            border: 2px solid #DAA520;
            box-shadow: 0 4px 20px rgba(218, 165, 32, 0.4);
        }

        .app-header {
            display: flex;
            align-items: start;
            gap: 15px;
            margin-bottom: 15px;
        }

        .app-icon {
            font-size: 3em;
        }

        .app-title {
            flex: 1;
        }

        .app-title h3 {
            color: white;
            font-size: 1.3em;
            margin-bottom: 8px;
        }

        .badges {
            display: flex;
            gap: 8px;
            flex-wrap: wrap;
        }

        .badge {
            padding: 4px 12px;
            border-radius: 15px;
            font-size: 0.75em;
            font-weight: bold;
        }

        .badge-free {
            background: rgba(218, 165, 32, 0.2);
            color: #FFD700;
            border: 1px solid rgba(218, 165, 32, 0.4);
        }

        .badge-both {
            background: rgba(218, 165, 32, 0.15);
            color: #DAA520;
            border: 1px solid rgba(218, 165, 32, 0.3);
        }

        .app-description {
            color: #ccc;
            margin-bottom: 15px;
            line-height: 1.6;
        }

        .features {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 15px;
        }

        .feature-tag {
            background: rgba(218, 165, 32, 0.15);
            color: #FFD700;
            padding: 5px 12px;
            border-radius: 12px;
            font-size: 0.8em;
            border: 1px solid rgba(218, 165, 32, 0.3);
        }

        .app-links {
            display: flex;
            gap: 10px;
        }

        .app-link {
            flex: 1;
            padding: 12px;
            border-radius: 12px;
            text-decoration: none;
            font-weight: bold;
            text-align: center;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        .link-web {
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
        }

        .link-app {
            background: linear-gradient(135deg, #B8860B 0%, #DAA520 100%);
            color: white;
        }

        .app-link:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 15px rgba(218, 165, 32, 0.4);
        }

        .note {
            background: rgba(218, 165, 32, 0.15);
            color: #FFD700;
            padding: 10px;
            border-radius: 8px;
            font-size: 0.85em;
            margin-top: 10px;
            border: 1px solid rgba(218, 165, 32, 0.3);
        }

        /* Tutorials */
        .tutorial-card {
            background: rgba(30, 30, 30, 0.95);
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 25px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            animation: fadeInUp 0.6s;
            border: 1px solid rgba(218, 165, 32, 0.2);
        }

        .tutorial-header {
            display: flex;
            gap: 20px;
            margin-bottom: 20px;
        }

        .tutorial-icon {
            font-size: 4em;
        }

        .tutorial-title h3 {
            color: white;
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .tutorial-desc {
            color: #ccc;
            line-height: 1.6;
        }

        .steps-box {
            background: rgba(218, 165, 32, 0.1);
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(218, 165, 32, 0.2);
        }

        .steps-box h4 {
            color: #FFD700;
            margin-bottom: 15px;
            font-size: 1.2em;
        }

        .step {
            display: flex;
            gap: 15px;
            margin-bottom: 15px;
            align-items: start;
        }

        .step-number {
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            flex-shrink: 0;
        }

        .step-text {
            color: white;
            line-height: 1.6;
            padding-top: 3px;
        }

        /* Interactive Tools */
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
            margin-bottom: 30px;
        }

        .tool-card {
            background: rgba(30, 30, 30, 0.95);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            transition: all 0.3s;
            border: 1px solid rgba(218, 165, 32, 0.2);
        }

        .tool-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(218, 165, 32, 0.3);
            border-color: rgba(218, 165, 32, 0.5);
        }

        .tool-icon {
            font-size: 4em;
            margin-bottom: 15px;
        }

        .tool-card h3 {
            color: white;
            margin-bottom: 15px;
            font-size: 1.3em;
        }

        .tool-card p {
            color: #ccc;
            margin-bottom: 20px;
            line-height: 1.6;
        }

        .tool-btn {
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
            border: none;
            padding: 15px 30px;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            width: 100%;
            transition: all 0.3s;
        }

        .tool-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 15px rgba(218, 165, 32, 0.4);
        }

        /* Tips */
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .tip-box {
            background: rgba(30, 30, 30, 0.95);
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(218, 165, 32, 0.2);
        }

        .tip-box h4 {
            margin-bottom: 15px;
            font-size: 1.2em;
        }

        .tip-box ul {
            list-style: none;
        }

        .tip-box li {
            color: white;
            margin-bottom: 8px;
            line-height: 1.6;
        }

        /* Footer */
        .footer {
            background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
            border-radius: 20px;
            padding: 40px;
            text-align: center;
            color: white;
            margin-top: 40px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
            border: 2px solid rgba(218, 165, 32, 0.3);
        }

        .footer h3 {
            font-size: 2em;
            margin-bottom: 15px;
        }

        .footer p {
            font-size: 1.2em;
            margin-bottom: 25px;
        }

        .footer-whatsapp {
            display: inline-flex;
            align-items: center;
            gap: 15px;
            background: linear-gradient(135deg, #DAA520 0%, #FFD700 100%);
            color: #1a1a1a;
            padding: 20px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.2em;
            box-shadow: 0 4px 15px rgba(218, 165, 32, 0.4);
            transition: all 0.3s;
        }

        .footer-whatsapp:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(218, 165, 32, 0.6);
        }

        /* Animations */
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .hidden {
            display: none;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2em;
            }
            
            .apps-grid {
                grid-template-columns: 1fr;
            }
            
            .tips-grid {
                grid-template-columns: 1fr;
            }
        }

        /* News Styles */
        .news-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 25px;
            margin-bottom: 40px;
        }

        .news-card {
            background: rgba(30, 30, 30, 0.95);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            transition: all 0.3s;
            animation: fadeInUp 0.6s;
            border: 1px solid rgba(218, 165, 32, 0.2);
        }

        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(218, 165, 32, 0.3);
            border-color: rgba(218, 165, 32, 0.5);
        }

        .news-image {
            width: 100%;
            height: 200px;
            background: linear-gradient(135deg, #DAA520 0%, #2d2d2d 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4em;
        }

        .news-content {
            padding: 25px;
        }

        .news-date {
            color: #999;
            font-size: 0.85em;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .news-title {
            color: white;
            font-size: 1.4em;
            font-weight: bold;
            margin-bottom: 15px;
            line-height: 1.4;
        }

        .news-description {
            color: #ccc;
            line-height: 1.6;
            margin-bottom: 15px;
        }

        .news-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 15px;
        }

        .news-tag {
            background: rgba(218, 165, 32, 0.15);
            color: #FFD700;
            padding: 5px 12px;
            border-radius: 12px;
            font-size: 0.8em;
            font-weight: bold;
            border: 1px solid rgba(218, 165, 32, 0.3);
        }

        .news-link {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            color: #FFD700;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
        }

        .news-link:hover {
            color: #DAA520;
            gap: 12px;
        }

        .breaking-badge {
            background: #dc3545;
            color: white;
            padding: 4px 12px;
            border-radius: 15px;
            font-size: 0.75em;
            font-weight: bold;
            display: inline-block;
            margin-bottom: 10px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% {
                opacity: 1;
            }
            50% {
                opacity: 0.7;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <h1>✨ الدليل الشامل للذكاء الاصطناعي ✨</h1>
            <p>أكثر من 35+ تطبيق وموقع AI 🚀</p>
            <a href="https://wa.me/201032135736" class="whatsapp-btn" target="_blank">
                📱 تواصل معنا على واتساب - جوكر لينك
            </a>
        </div>

        <!-- Tabs -->
        <div class="tabs">
            <button class="tab-btn active" onclick="showTab('apps')">🌐 التطبيقات والمواقع</button>
            <button class="tab-btn" onclick="showTab('tutorials')">📚 الشروحات</button>
            <button class="tab-btn" onclick="showTab('interactive')">⚡ أدوات تفاعلية</button>
            <button class="tab-btn" onclick="showTab('news')">📰 أخبار الذكاء الاصطناعي</button>
        </div>

        <!-- Apps Tab -->
        <div id="apps-tab">
            <!-- Categories -->
            <div class="categories">
                <button class="category-btn active" onclick="filterApps('all')">الكل</button>
                <button class="category-btn" onclick="filterApps('chat')">💬 مساعدات ذكية</button>
                <button class="category-btn" onclick="filterApps('image')">🎨 صور</button>
                <button class="category-btn" onclick="filterApps('video')">🎬 فيديو</button>
                <button class="category-btn" onclick="filterApps('language')">🌐 لغة</button>
                <button class="category-btn" onclick="filterApps('code')">💻 برمجة</button>
                <button class="category-btn" onclick="filterApps('voice')">🎤 صوت</button>
                <button class="category-btn" onclick="filterApps('writing')">✍️ كتابة</button>
            </div>

            <!-- Apps Grid -->
            <div class="apps-grid" id="apps-container"></div>
        </div>

        <!-- Tutorials Tab -->
        <div id="tutorials-tab" class="hidden">
            <div id="tutorials-container"></div>
        </div>

        <!-- Interactive Tab -->
        <div id="interactive-tab" class="hidden">
            <div class="tools-grid" id="tools-container"></div>
            
            <div style="background: linear-gradient(135deg, #e0c3fc 0%, #8ec5fc 100%); border-radius: 20px; padding: 30px; margin-top: 30px;">
                <h3 style="font-size: 1.8em; margin-bottom: 20px; color: #333;">🧠 نصائح سريعة للاستخدام الفعال</h3>
                <div class="tips-grid">
                    <div class="tip-box">
                        <h4 style="color: #667eea;">💡 للمبتدئين:</h4>
                        <ul>
                            <li>• ابدأ بأدوات سهلة مثل ChatGPT وCanva</li>
                            <li>• جرب استخدامات بسيطة أولاً</li>
                            <li>• لا تخف من التجربة والخطأ</li>
                            <li>• شاهد فيديوهات تعليمية على يوتيوب</li>
                        </ul>
                    </div>
                    <div class="tip-box">
                        <h4 style="color: #764ba2;">🚀 للمحترفين:</h4>
                        <ul>
                            <li>• ادمج أكثر من أداة معاً للنتائج الأفضل</li>
                            <li>• استخدم الـ APIs للأتمتة</li>
                            <li>• جرب النماذج المتقدمة والمدفوعة</li>
                            <li>• طور سير عمل خاص بك</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <!-- News Tab -->
        <div id="news-tab" class="hidden">
            <div style="text-align: center; margin-bottom: 30px;">
                <h2 style="font-size: 2.5em; color: white; margin-bottom: 10px;">📰 آخر أخبار الذكاء الاصطناعي</h2>
                <p style="color: white; font-size: 1.1em;">تابع أحدث التطورات والإصدارات في عالم AI</p>
            </div>
            <div class="news-grid" id="news-container"></div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <h3>هل تحتاج مساعدة؟</h3>
            <p>تواصل معنا للاستشارات والدعم الفني</p>
            <a href="https://wa.me/201032135736" class="footer-whatsapp" target="_blank">
                📱 واتساب: 01032135736 - جوكر لينك
            </a>
            <p style="margin-top: 25px; font-size: 0.9em; opacity: 0.9;">
                ✨ نحن هنا لمساعدتك في اختيار واستخدام أفضل أدوات الذكاء الاصطناعي ✨
            </p>
        </div>
    </div>

    <script>
        const apps = [
            {category: 'chat', name: 'ChatGPT', icon: '🤖', description: 'أقوى مساعد ذكي من OpenAI للإجابة والكتابة والبرمجة', features: ['إجابات ذكية', 'كتابة محتوى', 'مساعدة برمجية', 'شرح المفاهيم'], app: 'https://play.google.com/store/apps/details?id=com.openai.chatgpt', web: 'https://chat.openai.com', free: true},
            {category: 'chat', name: 'Claude', icon: '🧠', description: 'مساعد ذكي متطور من Anthropic للمحادثات العميقة والتحليل', features: ['محادثات طويلة', 'تحليل عميق', 'برمجة متقدمة'], app: 'https://play.google.com/store/apps/details?id=com.anthropic.claude', web: 'https://claude.ai', free: true},
            {category: 'chat', name: 'Google Gemini', icon: '✨', description: 'مساعد جوجل الذكي مع قدرات بحث وتحليل صور متقدمة', features: ['تحليل الصور', 'البحث المباشر', 'متكامل مع جوجل'], app: 'https://play.google.com/store/apps/details?id=com.google.android.apps.bard', web: 'https://gemini.google.com', free: true},
            {category: 'chat', name: 'Microsoft Copilot', icon: '💡', description: 'مساعد مايكروسوفت الذكي مع إمكانيات ChatGPT وDALL-E', features: ['دردشة ذكية', 'إنشاء صور', 'بحث متقدم'], app: 'https://play.google.com/store/apps/details?id=com.microsoft.copilot', web: 'https://copilot.microsoft.com', free: true},
            {category: 'chat', name: 'Perplexity AI', icon: '🔍', description: 'محرك بحث ذكي يجمع المعلومات ويقدم إجابات شاملة', features: ['بحث ذكي', 'مصادر موثوقة', 'إجابات دقيقة'], web: 'https://www.perplexity.ai', free: true},
            {category: 'image', name: 'Midjourney', icon: '🎨', description: 'أفضل أداة لإنشاء صور فنية احترافية بالذكاء الاصطناعي', features: ['جودة عالية جداً', 'صور فنية', 'واقعية مذهلة'], web: 'https://www.midjourney.com', free: false, note: 'يحتاج اشتراك'},
            {category: 'image', name: 'DALL-E 3', icon: '🖼️', description: 'مولد صور من OpenAI، متوفر عبر ChatGPT Plus وBing', features: ['دقة عالية', 'فهم النص', 'تفاصيل دقيقة'], web: 'https://openai.com/dall-e-3', free: true, note: 'مجاني عبر Bing'},
            {category: 'image', name: 'Leonardo.ai', icon: '🎭', description: 'إنشاء صور وأصول رقمية للألعاب والتصميم', features: ['صور الألعاب', 'أصول رقمية', 'أنماط متنوعة'], web: 'https://leonardo.ai', free: true},
            {category: 'image', name: 'Remini', icon: '📸', description: 'تحسين جودة الصور القديمة والمشوشة', features: ['تحسين الجودة', 'إصلاح الصور'], app: 'https://play.google.com/store/apps/details?id=com.remini', web: 'https://remini.ai', free: true, note: 'استخدامات يومية محدودة'},
            {category: 'image', name: 'PhotoRoom', icon: '✂️', description: 'إزالة الخلفية وتحرير الصور للمنتجات', features: ['إزالة خلفية', 'خلفيات جديدة'], app: 'https://play.google.com/store/apps/details?id=com.photoroom.app', web: 'https://www.photoroom.com', free: true},
            {category: 'image', name: 'Picsart', icon: '🖌️', description: 'محرر صور شامل مع أدوات AI قوية', features: ['تحرير شامل', 'فلاتر AI', 'تأثيرات فنية'], app: 'https://play.google.com/store/apps/details?id=com.picsart.studio', web: 'https://picsart.com', free: true},
            {category: 'image', name: 'Canva', icon: '🎨', description: 'تصميم جرافيك سهل مع أدوات AI متطورة', features: ['قوالب جاهزة', 'تصميم سهل', 'أدوات AI'], app: 'https://play.google.com/store/apps/details?id=com.canva.editor', web: 'https://www.canva.com', free: true},
            {category: 'video', name: 'CapCut', icon: '🎬', description: 'أفضل محرر فيديو مجاني بميزات AI متقدمة', features: ['مونتاج احترافي', 'إزالة خلفية', 'ترجمة تلقائية', 'بدون علامة مائية'], app: 'https://play.google.com/store/apps/details?id=com.lemon.lvoverseas', web: 'https://www.capcut.com', free: true, highlight: true},
            {category: 'video', name: 'Runway', icon: '🎥', description: 'أدوات فيديو AI متقدمة لإنشاء وتحرير الفيديوهات', features: ['Gen-2 للفيديو', 'إزالة خلفية', 'تأثيرات متقدمة'], web: 'https://runwayml.com', free: true},
            {category: 'video', name: 'Synthesia', icon: '🎭', description: 'إنشاء فيديوهات بمقدمين افتراضيين', features: ['مقدمين AI', 'لغات متعددة'], web: 'https://www.synthesia.io', free: false, note: 'يحتاج اشتراك'},
            {category: 'language', name: 'DeepL', icon: '🌐', description: 'أفضل مترجم بالذكاء الاصطناعي بترجمة طبيعية', features: ['ترجمة دقيقة', 'لغة طبيعية', '31 لغة'], app: 'https://play.google.com/store/apps/details?id=com.deepl.mobiletranslator', web: 'https://www.deepl.com', free: true},
            {category: 'language', name: 'Grammarly', icon: '✍️', description: 'مساعد كتابة ذكي لتحسين اللغة الإنجليزية', features: ['تصحيح نحوي', 'تحسين الأسلوب'], app: 'https://play.google.com/store/apps/details?id=com.grammarly.android.keyboard', web: 'https://www.grammarly.com', free: true},
            {category: 'language', name: 'QuillBot', icon: '📝', description: 'إعادة صياغة وتحسين النصوص بالذكاء الاصطناعي', features: ['إعادة صياغة', 'تلخيص', 'فحص القواعد'], web: 'https://quillbot.com', free: true},
            {category: 'code', name: 'GitHub Copilot', icon: '👨‍💻', description: 'مساعد برمجة ذكي من GitHub وOpenAI', features: ['إكمال الكود', 'اقتراحات ذكية'], web: 'https://github.com/features/copilot', free: false, note: 'اشتراك شهري'},
            {category: 'code', name: 'Codeium', icon: '⚡', description: 'إكمال كود ذكي مجاني للمطورين', features: ['مجاني بالكامل', '70+ لغة', 'سريع جداً'], web: 'https://codeium.com', free: true, highlight: true},
            {category: 'code', name: 'Replit AI', icon: '💻', description: 'بيئة برمجة ذكية مع مساعد AI', features: ['كتابة كود', 'شرح الكود', 'إصلاح الأخطاء'], web: 'https://replit.com', free: true},
            {category: 'voice', name: 'ElevenLabs', icon: '🎙️', description: 'أفضل أداة لتوليد الصوت بالذكاء الاصطناعي', features: ['أصوات واقعية', 'نسخ الصوت', 'لغات متعددة'], web: 'https://elevenlabs.io', free: true, note: '10,000 حرف مجاناً شهرياً'},
            {category: 'voice', name: 'Murf AI', icon: '🗣️', description: 'تحويل النص إلى صوت احترافي', features: ['أصوات طبيعية', 'لغات متعددة'], web: 'https://murf.ai', free: true},
            {category: 'writing', name: 'Copy.ai', icon: '📄', description: 'كتابة محتوى تسويقي ونصوص إعلانية', features: ['نصوص إعلانية', 'بوستات سوشيال'], web: 'https://www.copy.ai', free: true},
            {category: 'writing', name: 'Notion AI', icon: '📓', description: 'مساعد كتابة ذكي داخل Notion', features: ['كتابة وتحرير', 'تلخيص', 'ترجمة'], web: 'https://www.notion.so/product/ai', free: true}
        ];

        const tutorials = [
            {title: 'كيفية استخدام ChatGPT بفعالية', desc: 'تعلم كيف تكتب أفضل الأوامر (Prompts) للحصول على نتائج مذهلة', icon: '📚', steps: ['كن واضحاً ومحدداً في طلبك', 'استخدم أمثلة لتوضيح ما تريد', 'اطلب تنسيق معين للإجابة', 'اطلب من ChatGPT أن يسألك أسئلة توضيحية']},
            {title: 'إنشاء صور احترافية بالـ AI', desc: 'دليل شامل لكتابة أوامر فعالة لمولدات الصور', icon: '🎨', steps: ['حدد نوع الصورة (واقعية، فنية، كرتونية)', 'اذكر التفاصيل المهمة (الألوان، الإضاءة، الزاوية)', 'استخدم كلمات دقيقة ووصفية', 'جرب إضافة "4K, high quality, detailed" للجودة العالية']},
            {title: 'مونتاج الفيديو بالذكاء الاصطناعي', desc: 'كيف تستخدم CapCut وأدوات AI لعمل فيديوهات احترافية', icon: '🎬', steps: ['استورد الفيديو واستخدم Auto Captions', 'جرب Remove Background لإزالة الخلفية', 'استخدم AI Effects للتأثيرات الذكية', 'استعمل Text to Speech لإضافة تعليق صوتي']},
            {title: 'البرمجة باستخدام AI', desc: 'استخدم مساعدي البرمجة الأذكياء لكتابة كود أفضل', icon: '💻', steps: ['اشرح ما تريده بالتفصيل بلغة بسيطة', 'اطلب شرح الكود بعد كتابته', 'اطلب اقتراحات لتحسين الكود', 'استخدم AI لإيجاد وإصلاح الأخطاء']},
            {title: 'تحسين الكتابة والمحتوى', desc: 'استخدم أدوات AI لكتابة محتوى جذاب واحترافي', icon: '✍️', steps: ['ابدأ بفكرة عامة واطلب من AI توسيعها', 'استخدم Grammarly لتحسين القواعد', 'استعمل QuillBot لإعادة صياغة النصوص', 'اطلب من ChatGPT تحسين الأسلوب']}
        ];

        const tools = [
            {title: 'مولد أوامر الصور', desc: 'ساعدني في كتابة أمر احترافي لتوليد صورة', icon: '🎨'},
            {title: 'محسن النصوص', desc: 'أدخل نصك وسأحسنه لك بأساليب مختلفة', icon: '✨'},
            {title: 'مساعد اختيار الأداة', desc: 'أخبرني بما تريد عمله وسأقترح أفضل أداة', icon: '🎯'}
        ];

        const news = [
            {
                title: 'OpenAI تطلق GPT-5 بقدرات استدلال متقدمة',
                description: 'أعلنت OpenAI عن إطلاق الجيل الخامس من نماذجها اللغوية بتحسينات كبيرة في الفهم والاستدلال المنطقي والقدرة على حل المسائل المعقدة.',
                date: 'منذ 3 أيام',
                icon: '🤖',
                tags: ['ChatGPT', 'OpenAI', 'نماذج لغوية'],
                breaking: true
            },
            {
                title: 'Google تدمج Gemini في جميع خدماتها',
                description: 'جوجل تعلن عن دمج كامل لنموذج Gemini في Gmail و Google Docs و Google Sheets، مما يتيح للمستخدمين الاستفادة من AI مباشرة في أدوات العمل اليومية.',
                date: 'منذ 5 أيام',
                icon: '✨',
                tags: ['Google', 'Gemini', 'إنتاجية']
            },
            {
                title: 'Midjourney V7 يحقق واقعية غير مسبوقة',
                description: 'الإصدار السابع من Midjourney يقدم جودة صور فوتوغرافية مذهلة مع تحسينات كبيرة في التفاصيل والإضاءة وفهم الأوامر المعقدة.',
                date: 'منذ أسبوع',
                icon: '🎨',
                tags: ['Midjourney', 'توليد صور', 'فن رقمي']
            },
            {
                title: 'Meta تطلق Llama 4 مفتوح المصدر',
                description: 'ميتا تواصل دعم المجتمع المفتوح بإطلاق Llama 4، نموذج لغوي قوي ومجاني تماماً للاستخدام التجاري، منافساً لـ GPT-4.',
                date: 'منذ أسبوعين',
                icon: '🦙',
                tags: ['Meta', 'Llama', 'مفتوح المصدر']
            },
            {
                title: 'Anthropic تعلن عن Claude 4 بذاكرة طويلة المدى',
                description: 'Claude 4 يأتي بقدرة على تذكر المحادثات السابقة عبر الجلسات، وفهم سياق أعمق، ودعم ملفات أكبر حتى 1 مليون كلمة.',
                date: 'منذ أسبوعين',
                icon: '🧠',
                tags: ['Anthropic', 'Claude', 'ذاكرة طويلة']
            },
            {
                title: 'Sora من OpenAI متاح الآن للجميع',
                description: 'أداة توليد الفيديو من النص Sora أصبحت متاحة لجميع المستخدمين بعد فترة تجريبية، مع إمكانية إنشاء فيديوهات حتى دقيقة كاملة.',
                date: 'منذ 3 أسابيع',
                icon: '🎬',
                tags: ['OpenAI', 'Sora', 'توليد فيديو']
            },
            {
                title: 'ثورة في الترجمة الفورية بالذكاء الاصطناعي',
                description: 'أجهزة جديدة مدعومة بـ AI تترجم المحادثات فورياً بدقة 98% في أكثر من 100 لغة، مما يغير طريقة التواصل العالمي.',
                date: 'منذ شهر',
                icon: '🌐',
                tags: ['ترجمة', 'تواصل', 'تقنية']
            },
            {
                title: 'GitHub Copilot يتعلم من مشاريعك الخاصة',
                description: 'تحديث جديد يسمح لـ Copilot بالتعلم من أسلوب الكود الخاص بك ومشاريعك، مما يجعل الاقتراحات أكثر تخصيصاً ودقة.',
                date: 'منذ شهر',
                icon: '💻',
                tags: ['GitHub', 'Copilot', 'برمجة']
            },
            {
                title: 'AI يكتشف أدوية جديدة في أيام بدلاً من سنوات',
                description: 'باحثون يستخدمون الذكاء الاصطناعي لاكتشاف مركبات دوائية جديدة للسرطان في 21 يوماً فقط، عملية كانت تستغرق عشر سنوات.',
                date: 'منذ شهر',
                icon: '💊',
                tags: ['طب', 'أبحاث', 'صحة']
            },
            {
                title: 'ElevenLabs تطلق استنساخ صوت بـ 30 لغة',
                description: 'الآن يمكنك استنساخ صوتك والتحدث بـ 30 لغة مختلفة بنفس نبرتك وأسلوبك، فتحاً آفاق جديدة لصناع المحتوى.',
                date: 'منذ شهرين',
                icon: '🎙️',
                tags: ['ElevenLabs', 'صوت', 'لغات']
            },
            {
                title: 'Adobe Firefly يدمج AI في Photoshop بالكامل',
                description: 'تحديثات ثورية في Photoshop مع أدوات AI لإزالة الخلفيات، توسيع الصور، وإنشاء محتوى واقعي بأوامر نصية بسيطة.',
                date: 'منذ شهرين',
                icon: '🖼️',
                tags: ['Adobe', 'Photoshop', 'تصميم']
            },
            {
                title: 'روبوتات ذكية تساعد المسنين في المنازل',
                description: 'روبوتات مدعومة بالذكاء الاصطناعي بدأت العمل في دور الرعاية، تساعد المسنين في المهام اليومية وتوفر رفقة وتنبيهات طبية.',
                date: 'منذ شهرين',
                icon: '🤖',
                tags: ['روبوتات', 'رعاية صحية', 'مجتمع']
            }
        ];

        function renderApps(category = 'all') {
            const container = document.getElementById('apps-container');
            const filtered = category === 'all' ? apps : apps.filter(a => a.category === category);
            
            container.innerHTML = filtered.map(app => `
                <div class="app-card ${app.highlight ? 'highlight' : ''}">
                    <div class="app-header">
                        <div class="app-icon">${app.icon}</div>
                        <div class="app-title">
                            <h3>${app.name}</h3>
                            <div class="badges">
                                ${app.free ? '<span class="badge badge-free">مجاني</span>' : ''}
                                ${app.app && app.web ? '<span class="badge badge-both">ويب + تطبيق</span>' : ''}
                            </div>
                        </div>
                    </div>
                    <p class="app-description">${app.description}</p>
                    <div class="features">
                        ${app.features.map(f => `<span class="feature-tag">${f}</span>`).join('')}
                    </div>
                    ${app.note ? `<div class="note">⚠️ ${app.note}</div>` : ''}
                    <div class="app-links">
                        ${app.web ? `<a href="${app.web}" class="app-link link-web" target="_blank">🌐 الموقع</a>` : ''}
                        ${app.app ? `<a href="${app.app}" class="app-link link-app" target="_blank">📱 التطبيق</a>` : ''}
                    </div>
                </div>
            `).join('');
        }

        function renderTutorials() {
            const container = document.getElementById('tutorials-container');
            container.innerHTML = tutorials.map(t => `
                <div class="tutorial-card">
                    <div class="tutorial-header">
                        <div class="tutorial-icon">${t.icon}</div>
                        <div class="tutorial-title">
                            <h3>${t.title}</h3>
                            <p class="tutorial-desc">${t.desc}</p>
                        </div>
                    </div>
                    <div class="steps-box">
                        <h4>الخطوات:</h4>
                        ${t.steps.map((s, i) => `
                            <div class="step">
                                <div class="step-number">${i + 1}</div>
                                <div class="step-text">${s}</div>
                            </div>
                        `).join('')}
                    </div>
                </div>
            `).join('');
        }

        function renderTools() {
            const container = document.getElementById('tools-container');
            container.innerHTML = tools.map(t => `
                <div class="tool-card">
                    <div class="tool-icon">${t.icon}</div>
                    <h3>${t.title}</h3>
                    <p>${t.desc}</p>
                    <button class="tool-btn">جرب الآن</button>
                </div>
            `).join('');
        }

        function renderNews() {
            const container = document.getElementById('news-container');
            container.innerHTML = news.map(n => `
                <div class="news-card">
                    <div class="news-image">${n.icon}</div>
                    <div class="news-content">
                        ${n.breaking ? '<span class="breaking-badge">🔥 عاجل</span>' : ''}
                        <div class="news-date">🕒 ${n.date}</div>
                        <h3 class="news-title">${n.title}</h3>
                        <p class="news-description">${n.description}</p>
                        <div class="news-tags">
                            ${n.tags.map(tag => `<span class="news-tag">${tag}</span>`).join('')}
                        </div>
                        <a href="#" class="news-link">اقرأ المزيد ←</a>
                    </div>
                </div>
            `).join('');
        }

        function showTab(tab) {
            document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
            event.target.classList.add('active');
            
            document.getElementById('apps-tab').classList.toggle('hidden', tab !== 'apps');
            document.getElementById('tutorials-tab').classList.toggle('hidden', tab !== 'tutorials');
            document.getElementById('interactive-tab').classList.toggle('hidden', tab !== 'interactive');
            document.getElementById('news-tab').classList.toggle('hidden', tab !== 'news');
        }

        function filterApps(category) {
            document.querySelectorAll('.category-btn').forEach(b => b.classList.remove('active'));
            event.target.classList.add('active');
            renderApps(category);
        }

        // Initialize
        renderApps();
        renderTutorials();
        renderTools();
        renderNews();
    </script>
</body>
</html>