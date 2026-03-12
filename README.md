<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root {
            --bg-dark: #050505;
            --accent-blue: #00d2ff;
            --accent-purple: #9d50bb;
            --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(255, 255, 255, 0.1);
        }
        body {
            background-color: var(--bg-dark);
            color: #e0e0e0;
            font-family: 'Inter', -apple-system, sans-serif;
            padding: 2rem;
            background-image: 
                radial-gradient(circle at 2px 2px, rgba(255,255,255,0.05) 1px, transparent 0);
            background-size: 40px 40px;
        }
        .glass-card {
            background: var(--glass);
            backdrop-filter: blur(10px);
            border: 1px solid var(--border);
            border-radius: 16px;
            padding: 24px;
            transition: all 0.3s ease;
        }
        .glass-card:hover {
            border-color: var(--accent-blue);
            box-shadow: 0 0 20px rgba(0, 210, 255, 0.1);
        }
        .hero-text {
            background: linear-gradient(to right, var(--accent-blue), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 800;
        }
        .terminal-bar {
            height: 4px;
            width: 100%;
            background: linear-gradient(90deg, var(--accent-blue), var(--accent-purple));
            border-radius: 2px;
            margin-bottom: 20px;
        }
        .tech-tag {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 8px;
            padding: 4px 12px;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        .stat-img {
            border-radius: 12px;
            filter: grayscale(20%) brightness(90%);
            transition: filter 0.3s ease;
        }
        .stat-img:hover {
            filter: grayscale(0%) brightness(100%);
        }
    </style>
</head>
<body>

<div class="max-w-4xl mx-auto space-y-8">
    <!-- Header: Minimal & High Tech -->
    <div class="text-center space-y-4">
        <h1 class="text-5xl hero-text tracking-tight">ROHAN VENKATESHA</h1>
        <p class="text-lg text-gray-400 font-medium italic">Transforming complex logic into elegant architectural solutions.</p>
        
        <div class="flex justify-center gap-3 pt-2">
            <a href="https://www.linkedin.com/in/rohan-venkatesha/" target="_blank">
                <img src="https://img.shields.io/badge/Connect-LinkedIn-0077B5?style=for-the-badge&logo=linkedin" alt="LinkedIn">
            </a>
            <a href="https://github.com/rohanvenkatesha/" target="_blank">
                <img src="https://img.shields.io/badge/Follow-GitHub-181717?style=for-the-badge&logo=github" alt="GitHub">
            </a>
        </div>
    </div>

    <!-- Main Terminal Grid -->
    <div class="glass-card">
        <div class="terminal-bar"></div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <div class="space-y-4">
                <h3 class="text-xl font-bold flex items-center gap-2">
                    <span class="text-blue-400">01.</span> THE ENGINEER
                </h3>
                <p class="text-gray-400 leading-relaxed">
                    Software Engineer specializing in <span class="text-white">Distributed Systems</span> and <span class="text-white">Cloud Infrastructure</span>. 
                    I focus on building resilient backends that power modern user experiences.
                </p>
                <div class="grid grid-cols-2 gap-2 text-sm">
                    <div class="text-gray-500">▹ Location: <span class="text-gray-300">Bengaluru, IN</span></div>
                    <div class="text-gray-500">▹ Experience: <span class="text-gray-300">Software Engineering</span></div>
                    <div class="text-gray-500">▹ Status: <span class="text-green-400">Active</span></div>
                    <div class="text-gray-500">▹ Focus: <span class="text-gray-300">Scalability</span></div>
                </div>
            </div>
            <div class="space-y-4">
                <h3 class="text-xl font-bold flex items-center gap-2">
                    <span class="text-purple-400">02.</span> CORE ARSENAL
                </h3>
                <div class="flex flex-wrap gap-2">
                    <span class="tech-tag">Python</span>
                    <span class="tech-tag">C++</span>
                    <span class="tech-tag">JavaScript</span>
                    <span class="tech-tag">SQL</span>
                    <span class="tech-tag">Docker</span>
                    <span class="tech-tag">Kubernetes</span>
                    <span class="tech-tag">AWS</span>
                    <span class="tech-tag">GCP</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Metrics Section -->
    <div class="space-y-6">
        <h2 class="text-2xl font-black flex items-center gap-3">
            <span class="h-px bg-gray-800 flex-grow"></span>
            SYSTEM ANALYTICS
            <span class="h-px bg-gray-800 flex-grow"></span>
        </h2>
        
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
            <img src="https://github-readme-stats.vercel.app/api?username=rohanvenkatesha&theme=transparent&text_color=a9b1d6&title_color=7aa2f7&icon_color=7aa2f7&hide_border=true&include_all_commits=true" class="stat-img w-full">
            <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rohanvenkatesha&theme=transparent&text_color=a9b1d6&title_color=7aa2f7&hide_border=true&layout=compact" class="stat-img w-full">
        </div>
        
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=rohanvenkatesha&theme=transparent&stroke=7aa2f7&fire=7aa2f7&ring=7aa2f7&currStreakNum=a9b1d6&hide_border=true" class="stat-img w-full">
    </div>

    <!-- Projects / Focus -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <div class="glass-card text-center group">
            <div class="text-3xl mb-2">⚡</div>
            <div class="font-bold text-sm">Microservices</div>
            <div class="text-xs text-gray-500 mt-2">Designing decoupled architectures.</div>
        </div>
        <div class="glass-card text-center">
            <div class="text-3xl mb-2">🛡️</div>
            <div class="font-bold text-sm">DevOps</div>
            <div class="text-xs text-gray-500 mt-2">Hardening CI/CD pipelines.</div>
        </div>
        <div class="glass-card text-center">
            <div class="text-3xl mb-2">🛰️</div>
            <div class="font-bold text-sm">Cloud Native</div>
            <div class="text-xs text-gray-500 mt-2">Deploying at global scale.</div>
        </div>
    </div>

    <!-- Footer Quote -->
    <div class="pt-10 flex flex-col items-center space-y-6">
        <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=transparent&text_color=7aa2f7" class="opacity-60 hover:opacity-100 transition-opacity">
        <div class="text-center">
            <p class="text-xs tracking-widest text-gray-600 uppercase">Built for Performance • © 2026</p>
        </div>
    </div>
</div>

</body>
</html>
