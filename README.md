# first-project
简介仓库
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王明凯 - 工业设计师 | 产品设计 | 济南</title>
    <!-- SEO优化 -->
    <meta name="description" content="王明凯 - 工业设计专业在读，擅长产品造型设计、Rhino建模、Keyshot渲染，专注用户体验与功能性结合的工业设计创作">
    <meta name="keywords" content="王明凯,工业设计,Rhino,Photoshop,Keyshot,产品设计,济南工业设计师,在读学生">
    <!-- 外部资源 -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.0/font/bootstrap-icons.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- 自定义样式 -->
    <style>
        :root {
            --bg-color: #f8f9fa;
            --card-bg: #ffffff;
            --text-color: #333333;
            --primary-color: #2563eb;
            --secondary-color: #64748b;
            --accent-color: #0891b2;
            --success-color: #16a34a;
            --warning-color: #d97706;
            --shadow: 0 2px 8px rgba(0,0,0,0.08);
            --hover-shadow: 0 8px 24px rgba(0,0,0,0.12);
        }
        .dark-mode {
            --bg-color: #121212;
            --card-bg: #1e1e1e;
            --text-color: #e0e0e0;
            --primary-color: #3b82f6;
            --secondary-color: #94a3b8;
            --accent-color: #06b6d4;
            --success-color: #22c55e;
            --warning-color: #f59e0b;
            --shadow: 0 2px 8px rgba(0,0,0,0.3);
            --hover-shadow: 0 8px 24px rgba(0,0,0,0.4);
        }
        body {
            font-family: "Microsoft YaHei", "PingFang SC", sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            transition: all 0.3s ease;
            line-height: 1.7;
            padding-bottom: 20px;
        }
        .card {
            background-color: var(--card-bg);
            box-shadow: var(--shadow);
            border: none;
            border-radius: 12px;
            margin-bottom: 2rem;
            transition: all 0.3s ease;
        }
        .card:hover {
            box-shadow: var(--hover-shadow);
        }
        .card-header {
            border-bottom: 1px solid rgba(var(--secondary-color), 0.1);
            border-radius: 12px 12px 0 0 !important;
            background: linear-gradient(90deg, var(--primary-color)/5, var(--accent-color)/5);
            padding: 1.2rem 1.5rem;
        }
        .badge {
            padding: 0.6rem 0.8rem;
            font-size: 0.9rem;
            border-radius: 8px;
            margin: 0.2rem;
            border: none;
        }
        /* 技能进度条 */
        .skill-progress {
            height: 10px;
            border-radius: 5px;
            background-color: rgba(var(--secondary-color), 0.1);
            margin-bottom: 1.2rem;
            overflow: hidden;
        }
        .skill-progress-bar {
            height: 100%;
            border-radius: 5px;
            background: linear-gradient(90deg, var(--primary-color), var(--accent-color));
            transition: width 1s ease;
        }
        /* 作品集样式 */
        .portfolio-item {
            border-radius: 12px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            margin-bottom: 1.5rem;
            border: 1px solid rgba(var(--secondary-color), 0.1);
        }
        .portfolio-item:hover {
            transform: translateY(-8px);
            box-shadow: var(--hover-shadow);
        }
        .portfolio-item img {
            width: 100%;
            height: 220px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        .portfolio-item:hover img {
            transform: scale(1.05);
        }
        .portfolio-caption {
            padding: 1.2rem;
            background-color: var(--card-bg);
            border-top: 1px solid rgba(var(--secondary-color), 0.1);
        }
        /* 深色模式切换按钮 */
        .theme-switch {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 999;
            width: 45px;
            height: 45px;
            border-radius: 50%;
            background-color: var(--card-bg);
            box-shadow: var(--shadow);
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            border: 1px solid rgba(var(--secondary-color), 0.1);
        }
        /* 个人简介样式 */
        .intro-card {
            background: linear-gradient(135deg, var(--primary-color)/15, var(--accent-color)/15);
            border: none;
        }
        /* 表单样式 */
        .form-control {
            background-color: var(--card-bg);
            border: 1px solid rgba(var(--secondary-color), 0.2);
            color: var(--text-color);
            border-radius: 8px;
            padding: 0.8rem 1rem;
        }
        .form-control:focus {
            background-color: var(--card-bg);
            color: var(--text-color);
            border-color: var(--primary-color);
            box-shadow: 0 0 0 0.2rem var(--primary-color)/15;
        }
        /* 荣誉徽章 */
        .honor-badge {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            background: linear-gradient(90deg, var(--success-color)/10, var(--warning-color)/10);
            border: 1px solid var(--success-color)/20;
        }
        /* 空白区域填充 */
        .empty-state {
            padding: 3rem 2rem;
            text-align: center;
            color: var(--secondary-color);
            background-color: rgba(var(--secondary-color), 0.05);
            border-radius: 12px;
        }
        .empty-state i {
            font-size: 3rem;
            margin-bottom: 1rem;
            color: var(--primary-color)/70;
        }
        /* 服务范围模块 */
        .service-item {
            padding: 1.5rem;
            border-radius: 12px;
            background-color: rgba(var(--primary-color), 0.05);
            margin-bottom: 1rem;
            border: 1px solid rgba(var(--primary-color), 0.1);
        }
        /* 底部样式 */
        footer {
            margin-top: 3rem;
            background: linear-gradient(90deg, var(--primary-color), var(--accent-color));
            color: white;
            border-radius: 12px 12px 0 0;
        }
        /* 在校经历时间线样式 */
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -20px;
            top: 20px;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background-color: var(--primary-color);
        }
        .timeline-item {
            position: relative;
            padding-left: 20px;
        }
    </style>
</head>
<body>
    <!-- 深色模式切换按钮 -->
    <div class="theme-switch" id="themeSwitch">
        <<i class="bi bi-moon-fill" id="themeIcon" style="font-size: 1.2rem;"></</i>
    </div>

    <div class="container mt-5 mb-5">
        <!-- 头部个人信息 -->
        <div class="row mb-5 align-items-center">
            <div class="col-md-3 text-center mb-4 mb-md-0">
                <img src="https://via.placeholder.com/200/2563eb/ffffff?text=WK" alt="王明凯头像" 
                     class="rounded-circle img-thumbnail shadow" width="200" height="200">
            </div>
            <div class="col-md-9">
                <h1 class="display-4 fw-bold">王明凯</h1>
                <h2 class="text-muted mb-4">工业设计专业在读 | 产品造型设计 | 交互设计</h2>
                
                <!-- 核心联系方式 -->
                <div class="d-flex flex-wrap gap-4 mb-4">
                    <div><<i class="bi bi-envelope-fill text-primary me-2"></</i>2788214191@qq.com</div>
                    <div><<i class="bi bi-telephone-fill text-primary me-2"></</i>15688495253</div>
                    <div><<i class="bi bi-geo-alt-fill text-primary me-2"></</i>济南市历下区</div>
                    <div><<i class="bi bi-github text-primary me-2"></</i><a href="https://github.com/你的用户名" target="_blank" class="text-decoration-none text-primary">GitHub</a></div>
                </div>

                <!-- 个人标签 -->
                <div class="d-flex flex-wrap gap-2 mb-4">
                    <span class="badge bg-primary text-white">产品设计</span>
                    <span class="badge bg-success text-white">Rhino建模</span>
                    <span class="badge bg-info text-white">Keyshot渲染</span>
                    <span class="badge bg-warning text-white">用户体验</span>
                    <span class="badge bg-dark text-white">Python可视化</span>
                    <span class="badge bg-purple text-white">在校优秀学生</span>
                </div>
            </div>
        </div>

        <!-- 个人简介 -->
        <div class="card intro-card mb-5">
            <div class="card-body">
                <h3 class="card-title mb-3"><<i class="bi bi-person-circle text-primary"></</i> 个人简介</h3>
                <p class="fs-5">
                    山东建筑大学工业设计专业在读（2024级，预计2028年毕业），GPA 3.8/4.0（专业前5%），专注于消费类产品造型设计、人机交互与数字化设计工具应用。
                    具备扎实的设计理论基础与实践能力，擅长通过Rhino、Keyshot等工具实现设计方案的快速可视化，同时掌握Python编程技能，
                    可开发设计辅助工具提升工作效率。入学以来表现优异，多次荣获校级一等奖学金、优秀学生、优秀学生干部等荣誉，
                    具备出色的团队管理与跨部门协作能力，坚持以用户需求为核心，打造兼具功能性、美学与商业价值的工业设计作品。
                </p>
            </div>
        </div>

        <!-- 设计服务范围 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-handshake-fill text-primary"></</i> 设计服务范围</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col-md-4">
                        <div class="service-item">
                            <h5 class="text-primary mb-2"><<i class="bi bi-pencil-square"></</i> 产品造型设计</h5>
                            <p class="mb-0">消费电子、家居产品、文创产品、工业设备外观设计，兼顾美学与工艺可行性</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="service-item">
                            <h5 class="text-primary mb-2"><<i class="bi bi-cube"></</i> 3D建模与渲染</h5>
                            <p class="mb-0">Rhino高精度建模、Keyshot写实渲染、产品效果图制作、原型设计</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="service-item">
                            <h5 class="text-primary mb-2"><<i class="bi bi-mouse-fill"></</i> 交互设计</h5>
                            <p class="mb-0">产品操作界面设计、人机交互流程优化、用户体验调研与分析</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="service-item">
                            <h5 class="text-primary mb-2"><<i class="bi bi-code-slash"></</i> 设计工具开发</h5>
                            <p class="mb-0">Python自动化脚本、参数化建模工具、设计数据可视化分析</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="service-item">
                            <h5 class="text-primary mb-2"><<i class="bi bi-file-earmark-text"></</i> 设计咨询</h5>
                            <p class="mb-0">产品设计策略、材料工艺选型、竞品分析、设计流程优化</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="service-item">
                            <h5 class="text-primary mb-2"><<i class="bi bi-lightbulb"></</i> 创新设计</h5>
                            <p class="mb-0">概念产品设计、可持续设计、产学研结合设计方案落地</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- 设计理念 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-lightbulb-fill text-primary"></</i> 设计理念</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col-md-6 mb-4">
                        <div class="p-3 border rounded bg-white/50 dark:bg-gray-800/50">
                            <h5 class="text-primary mb-2"><<i class="bi bi-handshake-angle"></</i> 以人为本</h5>
                            <p>设计的核心是解决用户需求，所有设计决策均基于用户调研与行为分析，确保产品符合人体工程学与使用习惯，让设计服务于人。</p>
                        </div>
                    </div>
                    <div class="col-md-6 mb-4">
                        <div class="p-3 border rounded bg-white/50 dark:bg-gray-800/50">
                            <h5 class="text-primary mb-2"><<i class="bi bi-recycle"></</i> 可持续设计</h5>
                            <p>注重环保材料与工艺的应用，在设计阶段考虑产品全生命周期，减少资源消耗与环境影响，践行绿色设计理念。</p>
                        </div>
                    </div>
                    <div class="col-md-6 mb-4">
                        <div class="p-3 border rounded bg-white/50 dark:bg-gray-800/50">
                            <h5 class="text-primary mb-2"><<i class="bi bi-puzzle-fill"></</i> 功能与美学统一</h5>
                            <p>拒绝为了造型牺牲功能，也不忽视美学价值，追求形式服务于功能的同时具备视觉吸引力，让产品既有实用性又有温度。</p>
                        </div>
                    </div>
                    <div class="col-md-6 mb-4">
                        <div class="p-3 border rounded bg-white/50 dark:bg-gray-800/50">
                            <h5 class="text-primary mb-2"><<i class="bi bi-arrow-up-right-dots"></</i> 创新驱动</h5>
                            <p>持续关注行业前沿技术与趋势，将新技术、新材料融入设计，探索产品的创新可能性，打造差异化的设计方案。</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- 教育背景 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-graduation-cap text-primary"></</i> 教育背景</h3>
            </div>
            <div class="card-body">
                <div class="timeline-item border rounded p-4 mb-3 bg-white/50 dark:bg-gray-800/50">
                    <div class="d-flex justify-content-between align-items-center mb-2">
                        <h5 class="mb-0">山东建筑大学</h5>
                        <span class="badge bg-secondary text-white">2024.09 - 2028.06（预计）</span>
                    </div>
                    <h6 class="text-primary">工业设计 | 本科 | 学士学位（预计）</h6>
                    <div class="mt-2">
                        <p><strong>核心课程：</strong>产品设计、人机工程学、工业设计史、造型基础、CAD/CAM、材料与工艺、交互设计、设计心理学、产品创新设计、设计素描、色彩构成</p>
                        <p><strong>学业成果：</strong>GPA 3.8/4.0（专业前5%），2024-2025学年荣获校级一等奖学金、校级优秀学生；2025-2026学年获评校级优秀学生干部</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- 技能矩阵 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-tools text-primary"></</i> 技能矩阵</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <!-- 设计软件技能 -->
                    <div class="col-md-6 mb-4">
                        <h4 class="mb-3 text-secondary"><<i class="bi bi-palette"></</i> 设计软件</h4>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>Rhino（建模）</span>
                                <span>95%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 95%"></div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>Keyshot（渲染）</span>
                                <span>90%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 90%"></div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>Photoshop（后期）</span>
                                <span>85%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 85%"></div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>Figma（交互设计）</span>
                                <span>75%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 75%"></div>
                            </div>
                        </div>
                    </div>

                    <!-- 编程与其他技能 -->
                    <div class="col-md-6 mb-4">
                        <h4 class="mb-3 text-secondary"><<i class="bi bi-code"></</i> 编程与其他</h4>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>Python（设计工具开发）</span>
                                <span>80%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 80%"></div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>产品调研与分析</span>
                                <span>90%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 90%"></div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>手绘草图</span>
                                <span>85%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 85%"></div>
                            </div>
                        </div>
                        <div class="mb-3">
                            <div class="d-flex justify-content-between mb-1">
                                <span>团队管理与沟通</span>
                                <span>95%</span>
                            </div>
                            <div class="skill-progress">
                                <div class="skill-progress-bar" style="width: 95%"></div>
                            </div>
                        </div>
                    </div>

                    <!-- 软技能标签 -->
                    <div class="col-12">
                        <h4 class="mb-3 text-secondary"><<i class="bi bi-people"></</i> 综合能力</h4>
                        <div class="d-flex flex-wrap">
                            <span class="badge bg-info text-white">用户研究</span>
                            <span class="badge bg-info text-white">设计思维</span>
                            <span class="badge bg-info text-white">团队协作</span>
                            <span class="badge bg-info text-white">问题解决</span>
                            <span class="badge bg-info text-white">项目管理</span>
                            <span class="badge bg-info text-white">快速原型</span>
                            <span class="badge bg-info text-white">竞品分析</span>
                            <span class="badge bg-info text-white">演讲汇报</span>
                            <span class="badge bg-info text-white">跨部门协作</span>
                            <span class="badge bg-info text-white">设计评审</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- 作品集展示 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-images text-primary"></</i> 设计作品集</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <!-- 作品1 -->
                    <div class="col-md-4">
                        <div class="portfolio-item">
                            <img src="https://via.placeholder.com/600/400?text=便携水杯设计" alt="便携水杯设计">
                            <div class="portfolio-caption">
                                <h5 class="fw-bold">便携环保水杯设计</h5>
                                <p class="text-muted small">
                                    设计理念：基于人体工程学的便携水杯，采用可降解PLA材料，兼顾握持舒适度与环保性，
                                    内置可拆卸滤网设计满足茶饮、咖啡等多场景使用需求，获校级设计大赛一等奖。
                                </p>
                                <div class="d-flex gap-2 mt-2">
                                    <span class="badge bg-secondary small">Rhino建模</span>
                                    <span class="badge bg-secondary small">Keyshot渲染</span>
                                    <span class="badge bg-secondary small">用户调研</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- 作品2 -->
                    <div class="col-md-4">
                        <div class="portfolio-item">
                            <img src="https://via.placeholder.com/600/400?text=办公椅设计" alt="人体工学办公椅设计">
                            <div class="portfolio-caption">
                                <h5 class="fw-bold">人体工学办公椅设计</h5>
                                <p class="text-muted small">
                                    设计理念：针对久坐办公人群的健康需求，优化腰托与头枕的可调节结构，
                                    采用透气3D网布材质，通过100+用户测试优化座椅角度，降低久坐疲劳感。
                                </p>
                                <div class="d-flex gap-2 mt-2">
                                    <span class="badge bg-secondary small">人机工程学</span>
                                    <span class="badge bg-secondary small">手绘草图</span>
                                    <span class="badge bg-secondary small">原型制作</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- 作品3 -->
                    <div class="col-md-4">
                        <div class="portfolio-item">
                            <img src="https://via.placeholder.com/600/400?text=智能家居控制器" alt="智能家居控制器设计">
                            <div class="portfolio-caption">
                                <h5 class="fw-bold">智能家居控制器设计</h5>
                                <p class="text-muted small">
                                    设计理念：一体化智能家居控制终端，极简的交互界面设计，适配多种家居风格，
                                    支持语音与触控双重操作，通过Python开发简易控制脚本实现设备联动。
                                </p>
                                <div class="d-flex gap-2 mt-2">
                                    <span class="badge bg-secondary small">交互设计</span>
                                    <span class="badge bg-secondary small">Figma</span>
                                    <span class="badge bg-secondary small">Python开发</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- 作品集更多按钮 -->
                <div class="text-center mt-4">
                    <a href="#" class="btn btn-primary px-4 py-2 rounded-pill">
                        <<i class="bi bi-arrow-right"></</i> 查看更多作品
                    </a>
                </div>
            </div>
        </div>

        <!-- 项目与实习经历 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-diagram-project text-primary"></</i> 项目与实习经历</h3>
            </div>
            <div class="card-body">
                <!-- 校园项目1 -->
                <div class="border rounded p-4 mb-4 bg-white/50 dark:bg-gray-800/50">
                    <h5 class="fw-bold">校园文创产品设计项目 | 团队负责人</h5>
                    <div class="text-muted mb-2">2025.03 - 2025.06 | 山东建筑大学</div>
                    <p><strong>项目描述：</strong>为学校125周年校庆设计系列文创产品（笔记本、书签、水杯、文创礼盒等），结合学校建筑特色与文化元素，兼顾实用性与纪念价值。</p>
                    <p><strong>我的职责：</strong></p>
                    <ul class="list-group list-group-flush mb-2">
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 组建5人设计团队，制定项目计划与分工，担任团队负责人</li>
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 主导用户调研（师生、校友），发放问卷300+份，确定目标用户需求与偏好</li>
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 完成核心产品的造型设计与3D建模，制作10+张渲染效果图与产品手册</li>
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 协调学校文创中心完成样品制作与展示，组织3场设计方案评审会</li>
                    </ul>
                    <p><strong>项目成果：</strong>设计方案被学校采用，制作首批2000套文创产品用于校庆纪念，获校级设计竞赛一等奖，个人获评优秀项目负责人</p>
                </div>

                <!-- 个人项目 -->
                <div class="border rounded p-4 mb-4 bg-white/50 dark:bg-gray-800/50">
                    <h5 class="fw-bold">设计辅助工具开发 | 个人项目</h5>
                    <div class="text-muted mb-2">2025.09 - 2025.12</div>
                    <p><strong>项目描述：</strong>针对工业设计中重复性建模工作，开发Python脚本工具，实现设计参数的快速计算、模型文件批量处理、渲染参数自动化设置。</p>
                    <p><strong>技术实现：</strong>使用Python + RhinoPython脚本，对接Rhino API，开发参数化建模模块；结合OpenCV实现设计草图的快速数字化处理。</p>
                    <p><strong>项目成果：</strong>将重复性建模工作时间缩短60%，脚本已分享给校内设计专业师生使用，累计下载超500次，获校级创新创业大赛二等奖</p>
                </div>

                <!-- 实习经历 -->
                <div class="border rounded p-4 bg-white/50 dark:bg-gray-800/50">
                    <h5 class="fw-bold">工业设计实习生 | 济南XX工业设计有限公司</h5>
                    <div class="text-muted mb-2">2026.07 - 2026.09 | 产品设计部</div>
                    <p><strong>工作内容：</strong></p>
                    <ul class="list-group list-group-flush mb-2">
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 协助设计师完成3款家居产品的外观设计，输出20+张手绘草图与Rhino建模文件</li>
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 使用Keyshot完成15+张产品渲染图，制作产品宣传册，优化渲染参数提升效率30%</li>
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 参与2个用户调研项目，整理竞品分析报告5份，为设计决策提供数据支持</li>
                        <li class="list-group-item bg-transparent border-0 ps-0">✓ 跟进产品打样流程，与工厂沟通工艺细节，解决3个建模与生产的衔接问题</li>
                    </ul>
                    <p><strong>实习成果：</strong>参与的2款水杯设计方案被客户采纳，优化的渲染流程在团队内推广使用，获"优秀实习生"称号</p>
                </div>
            </div>
        </div>

        <!-- 获奖与证书 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-award text-primary"></</i> 获奖与证书</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col-md-6 mb-3">
                        <div class="border rounded p-3 honor-badge">
                            <<i class="bi bi-trophy text-warning"></</i>
                            <div>
                                <h6 class="fw-bold mb-0">校级工业设计创新大赛 一等奖</h6>
                                <p class="text-muted small mb-0">2025年 | 山东建筑大学</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 mb-3">
                        <div class="border rounded p-3 honor-badge">
                            <<i class="bi bi-trophy text-warning"></</i>
                            <div>
                                <h6 class="fw-bold mb-0">校级一等奖学金</h6>
                                <p class="text-muted small mb-0">2024-2025、2025-2026学年（在读期间）</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 mb-3">
                        <div class="border rounded p-3 honor-badge">
                            <<i class="bi bi-trophy text-warning"></</i>
                            <div>
                                <h6 class="fw-bold mb-0">校级优秀学生</h6>
                                <p class="text-muted small mb-0">2024-2025学年</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 mb-3">
                        <div class="border rounded p-3 honor-badge">
                            <<i class="bi bi-trophy text-warning"></</i>
                            <div>
                                <h6 class="fw-bold mb-0">校级优秀学生干部</h6>
                                <p class="text-muted small mb-0">2025-2026学年</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 mb-3">
                        <div class="border rounded p-3 honor-badge">
                            <<i class="bi bi-certificate text-primary"></</i>
                            <div>
                                <h6 class="fw-bold mb-0">计算机二级（Python）</h6>
                                <p class="text-muted small mb-0">2025年 | 国家计算机等级考试</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 mb-3">
                        <div class="border rounded p-3 honor-badge">
                            <<i class="bi bi-certificate text-primary"></</i>
                            <div>
                                <h6 class="fw-bold mb-0">校级创新创业大赛 二等奖</h6>
                                <p class="text-muted small mb-0">2025年 | 山东建筑大学</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- 在校实践经历（新增，填充空白） -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-people-fill text-primary"></</i> 在校实践经历</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col-md-6 mb-4">
                        <div class="border rounded p-4 bg-white/50 dark:bg-gray-800/50">
                            <h5 class="fw-bold mb-2">工业设计系学生会 副主席</h5>
                            <div class="text-muted mb-2">2025.09 - 2026.09</div>
                            <ul class="list-group list-group-flush mb-2">
                                <li class="list-group-item bg-transparent border-0 ps-0">✓ 组织"设计之星"校园设计大赛，吸引全校200+学生参与</li>
                                <li class="list-group-item bg-transparent border-0 ps-0">✓ 协调举办3场行业设计师讲座，搭建学生与行业的沟通桥梁</li>
                                <li class="list-group-item bg-transparent border-0 ps-0">✓ 管理学生会10人团队，制定工作计划与考核制度，提升团队执行力</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-md-6 mb-4">
                        <div class="border rounded p-4 bg-white/50 dark:bg-gray-800/50">
                            <h5 class="fw-bold mb-2">设计工作室 核心成员</h5>
                            <div class="text-muted mb-2">2024.10 - 至今</div>
                            <ul class="list-group list-group-flush mb-2">
                                <li class="list-group-item bg-transparent border-0 ps-0">✓ 参与校企合作项目，为本地企业提供产品设计咨询服务</li>
                                <li class="list-group-item bg-transparent border-0 ps-0">✓ 负责工作室3D打印机、扫描仪等设备的日常管理与维护</li>
                                <li class="list-group-item bg-transparent border-0 ps-0">✓ 指导低年级学生Rhino建模与Keyshot渲染技能，累计开展5场培训</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- 联系方式表单 -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-envelope text-primary"></</i> 联系我</h3>
            </div>
            <div class="card-body">
                <form>
                    <div class="row mb-3">
                        <div class="col-md-6">
                            <label for="name" class="form-label">姓名</label>
                            <input type="text" class="form-control" id="name" placeholder="请输入您的姓名">
                        </div>
                        <div class="col-md-6">
                            <label for="email" class="form-label">邮箱</label>
                            <input type="email" class="form-control" id="email" placeholder="请输入您的邮箱">
                        </div>
                    </div>
                    <div class="mb-3">
                        <label for="subject" class="form-label">主题</label>
                        <input type="text" class="form-control" id="subject" placeholder="设计合作 / 实习咨询 / 项目交流 / 校园合作">
                    </div>
                    <div class="mb-3">
                        <label for="message" class="form-label">留言内容</label>
                        <textarea class="form-control" id="message" rows="5" placeholder="请输入您想沟通的内容..."></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary px-4 py-2 rounded-pill">
                        <<i class="bi bi-paper-plane"></</i> 发送留言
                    </button>
                </form>
            </div>
        </div>

        <!-- 职业规划（优化空白区域） -->
        <div class="card mb-5">
            <div class="card-header">
                <h3><<i class="bi bi-compass text-primary"></</i> 职业规划</h3>
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col-md-6">
                        <div class="empty-state">
                            <<i class="bi bi-rocket"></</i>
                            <h4 class="mb-2">在校期间目标（2024-2028）</h4>
                            <ul class="text-start mt-3">
                                <li>✓ 保持GPA前5%，争取获得国家级奖学金</li>
                                <li>✓ 参与2-3个国家级设计竞赛，积累获奖经历</li>
                                <li>✓ 完成2次行业顶尖企业实习，提升实战能力</li>
                                <li>✓ 发表1-2篇设计相关学术论文或专利</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="empty-state">
                            <<i class="bi bi-briefcase"></</i>
                            <h4 class="mb-2">毕业后规划（2028+）</h4>
                            <ul class="text-start mt-3">
                                <li>✓ 加入专业工业设计公司，从设计师助理成长为资深设计师</li>
                                <li>✓ 专注消费电子或家居产品领域，打造个人设计代表作</li>
                                <li>✓ 持续学习数字化设计技术，探索AI+设计的创新应用</li>
                                <li>✓ 长期目标：成为兼具设计能力与商业思维的设计总监</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- 底部版权信息 -->
    <footer class="py-5">
        <div class="container text-center">
            <p class="mb-0 fs-5">© 2024-2028 王明凯 - 工业设计专业在读</p>
            <p class="mb-0 small mt-2">专注于产品设计 | 所有设计作品均为原创 | 持续学习与创新</p>
            <div class="mt-3">
                <a href="mailto:2788214191@qq.com" class="text-white mx-2"><<i class="bi bi-envelope"></</i></a>
                <a href="https://github.com/你的用户名" target="_blank" class="text-white mx-2"><<i class="bi bi-github"></</i></a>
                <a href="tel:15688495253" class="text-white mx-2"><<i class="bi bi-telephone"></</i></a>
            </div>
        </div>
    </footer>

    <!-- 脚本 -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        // 深色模式切换
        const themeSwitch = document.getElementById('themeSwitch');
        const themeIcon = document.getElementById('themeIcon');
        const body = document.body;

        // 检查本地存储的主题偏好
        if (localStorage.getItem('theme') === 'dark') {
            body.classList.add('dark-mode');
            themeIcon.classList.remove('bi-moon-fill');
            themeIcon.classList.add('bi-sun-fill');
        }

        // 切换主题
        themeSwitch.addEventListener('click', () => {
            body.classList.toggle('dark-mode');
            if (body.classList.contains('dark-mode')) {
                localStorage.setItem('theme', 'dark');
                themeIcon.classList.remove('bi-moon-fill');
                themeIcon.classList.add('bi-sun-fill');
            } else {
                localStorage.setItem('theme', 'light');
                themeIcon.classList.remove('bi-sun-fill');
                themeIcon.classList.add('bi-moon-fill');
            }
        });

        // 表单提交提示
        document.querySelector('form').addEventListener('submit', (e) => {
            e.preventDefault();
            alert('留言提交成功！我会在24小时内回复您的邮件。');
            document.querySelector('form').reset();
        });

        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // 技能进度条动画
        window.addEventListener('scroll', () => {
            const skillBars = document.querySelectorAll('.skill-progress-bar');
            skillBars.forEach(bar => {
                const rect = bar.parentElement.getBoundingClientRect();
                if (rect.top < window.innerHeight - 100) {
                    bar.style.width = bar.style.width;
                }
            });
        });

        // 初始化进度条动画
        window.dispatchEvent(new Event('scroll'));
    </script>
</body>
</html>

