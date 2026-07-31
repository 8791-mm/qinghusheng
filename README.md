<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>清湖省MTR讨论官网</title>
    <style>
        /* 全局基础样式重置 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* 页面整体样式 */
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }

        /* 头部导航栏样式 */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: #fff;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            z-index: 1000;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        /* 导航栏标题样式 */
        header h1 {
            font-size: 1.2rem;
            color: #007bff;
        }

        /* 导航链接样式 */
        nav a {
            margin: 0 1rem;
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #007bff;
        }

        /* 主视觉区域（Hero Section）样式 */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            padding: 0 2rem;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            max-width: 600px;
        }

        /* 按钮样式 */
        .btn {
            background-color: #fff;
            color: #764ba2;
            padding: 0.8rem 2rem;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .btn:hover {
            transform: translateY(-3px);
        }

        /* 通用区块样式 */
        section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        section h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            text-align: center;
            color: #007bff;
        }

        /* 关于我区块样式 */
        .about p {
            text-align: center;
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto;
        }

        /* 项目展示区块样式 */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        /* 项目卡片样式 */
        .project-card {
            background-color: #fff;
            border-radius: 10px;
            padding: 2rem;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-5px);
        }

        .project-card h3 {
            color: #007bff;
            margin-bottom: 1rem;
        }

        /* 联系区块样式 */
        .contact {
            text-align: center;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        .contact p {
            font-size: 1.1rem;
            margin: 1rem 0;
        }

        /* 页脚样式 */
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 2rem;
            margin-top: 3rem;
        }

        /* 响应式适配（移动端） */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                padding: 1rem;
            }

            nav {
                margin-top: 1rem;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <!-- 头部导航区域 -->
    <header>
        <h1>清湖省MTR讨论官网 </h1>
        <nav>
            <a href="#home">首页</a>
            <a href="#about">关于我们</a>
            <a href="#projects">我们的项目</a>
            <a href="#contact">联系</a>
        </nav>
    </header>

    <!-- 主视觉区域 -->
    <section class="hero" id="home">
        <h2>欢迎来到清湖省MTR讨论官网</h2>
        <p>这是一个展示我们的作品、想法和服务器的地方，希望你能在这里找到感兴趣的内容，有更好的游览体验。</p>
        <a href="#about" class="btn">了解更多</a>
    </section>

    <!-- 关于我区块 -->
    <section class="about" id="about">
        <h2>关于我们</h2>
        <p>此网站为清湖省MTR服务器及同运营服务器交流群的网站，只负责群中一些小型事务办理</p>
<section class="projects">
    <h2>我们的项目</h2>
    <div class="projects-grid">
        <div class="project-card">
            <h3>清湖省MTR服务器内部建筑展示</h3>
            <p>可以直接观赏服务器建筑哦</p>
            <a href="about:blank" target="_blank" class="btn">查看详情</a>
        </div>
        <div class="project-card">
            <h3>玩家交流平台</h3>
            <p>玩家分享游戏攻略、交流玩法心得的在线论坛</p>
            <a href="about:blank" target="_blank" class="btn">进入论坛</a>
        </div>
        <div class="project-card" id="post-platform" style="display:none; grid-column: 1 / -1; background: linear-gradient(135deg, #f5f7fa 0%, #e4e8eb 100%);">
            <h3 style="color: #764ba2; margin-bottom: 1rem;">📝 玩家发帖平台</h3>
            <div class="post-form" style="background:#fff; padding:1.5rem; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.08);">
                <textarea id="postContent" placeholder="分享你的想法、交流心得...支持文字、表情、图片、视频！" style="width:100%; min-height:120px; padding:1rem; border:1px solid #ddd; border-radius:8px; resize:vertical; font-size:1rem; font-family:inherit; margin-bottom:1rem;"></textarea>
                
               
            <h3>服务器地图</h3>
            <p>可以直接观赏服务器平面地图哦</p>
            <a href="about:blank" target="_blank" class="btn">前往下载</a>
        </div>
    </div>
</section>

    <!-- 避雷挂人区块 -->
    <section class="projects" id="warning">
        <h2>避雷挂人专栏</h2>
        <div class="projects-grid">
            <div class="project-card">
                <h3>违规行为曝光</h3>
                <p>曝光服务器内的违规行为，维护良好的游戏环境</p>
                <a href="about:blank" target="_blank" class="btn">查看详情</a>
            </div>
            <div class="project-card">
                <h3>诈骗玩家名单</h3>
                <p>记录服务器中存在诈骗行为的玩家，提醒大家注意防范</p>
                <a href="about:blank" target="_blank" class="btn">查看名单</a>
            </div>
            <div class="project-card">
                <h3>恶意破坏他人建筑</h3>
                <p>曝光恶意破坏他人建筑的行为，保护玩家劳动成果</p>
                <a href="about:blank" target="_blank" class="btn">查看详情</a>
            </div>
        </div>
    </section>
    </section>



    <!-- 联系区块 -->
    <section class="contact" id="contact">
        <h2>联系我</h2>
        <p>如果你有任何合作想法或问题，欢迎通过以下方式联系我：</p>
        <p>📧 邮箱：example@email.com</p>
        <p>📱 微信：my_wechat</p>
    </section>

    <!-- 页脚区域 -->
    <footer>
        <p>© 2024 清湖省MTR讨论官网. 保留所有权利.</p>
    </footer>
</body>
</html>
        <p
