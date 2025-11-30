# WC-AI
<!DOCTYPE html>
<html lang="sw">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SynapseOS Console | Worldclass-AI</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Rangi Maalum za WC-AI (Deep Blue & AI Teal) */
        :root {
            --primary-bg: #0F172A; /* Slate 900 */
            --secondary-color: #2DD4BF; /* Teal 400 - AI Accent */
            --card-bg: #1E293B; /* Slate 800 */
        }
        body { background-color: var(--primary-bg); }
        .card { background-color: var(--card-bg); border-left: 4px solid var(--secondary-color); }
        .ai-status-active { color: #10B981; } /* Green */
        .ai-status-alert { color: #F59E0B; } /* Amber */
        .ai-status-risk { color: #EF4444; } /* Red */
    </style>
</head>

<body class="text-white">
    <div class="flex h-screen">
        
        <aside class="w-64 bg-slate-900 p-6 shadow-2xl">
            <h1 class="text-2xl font-bold mb-8" style="color:var(--secondary-color);">Synapse<span class="text-white">OS</span></h1>
            <nav class="space-y-4">
                <a href="#" class="flex items-center space-x-3 p-3 rounded-lg bg-slate-800 text-teal-400 font-medium">
                    <span>🏠</span> <span>Dashboard</span>
                </a>
                <a href="#" class="flex items-center space-x-3 p-3 rounded-lg hover:bg-slate-700">
                    <span>💾</span> <span>SynapseDB Core</span>
                </a>
                <a href="#" class="flex items-center space-x-3 p-3 rounded-lg hover:bg-slate-700">
                    <span>🔐</span> <span>SynapseAuth (IAM)</span>
                </a>
                <a href="#" class="flex items-center space-x-3 p-3 rounded-lg hover:bg-slate-700">
                    <span>🚨</span> <span>SynapseLogs & Alerts</span>
                </a>
                <a href="#" class="flex items-center space-x-3 p-3 rounded-lg hover:bg-slate-700">
                    <span>🤖</span> <span>AI Hubs & Automation</span>
                </a>
                <a href="#" class="flex items-center space-x-3 p-3 rounded-lg hover:bg-slate-700">
                    <span>🧾</span> <span>SynapseAudit (Compliance)</span>
                </a>
            </nav>
        </aside>

        <main class="flex-1 p-10 overflow-y-auto">
            <header class="mb-10 flex justify-between items-center">
                <h2 class="text-3xl font-semibold">Dashboard ya Mfumo</h2>
                <div class="flex items-center space-x-4">
                    <span class="text-sm font-light">Mtumiaji: Admin (WC-AI License)</span>
                    <button class="bg-teal-600 hover:bg-teal-700 text-white font-bold py-2 px-4 rounded-lg">
                        Toka (Logout)
                    </button>
                </div>
            </header>

            <section class="mb-12">
                <h3 class="text-xl font-medium mb-4 border-b border-slate-700 pb-2">🌐 Hali ya Core Services (Rust)</h3>
                <div class="grid grid-cols-1 md:grid-cols-4 gap-6">
                    
                    <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">SynapseDB Core</p>
                        <p class="text-3xl font-extrabold text-green-400">UP</p>
                        <p class="text-sm text-slate-400">Latency: <span class="text-green-400">1.2ms</span> (Rust Fast)</p>
                    </div>

                    <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">SynapseCache</p>
                        <p class="text-3xl font-extrabold text-green-400">UP</p>
                        <p class="text-sm text-slate-400">Hit Rate: <span class="text-yellow-400">98.5%</span></p>
                    </div>

                    <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">SynapseOS Controller</p>
                        <p class="text-3xl font-extrabold text-green-400">UP</p>
                        <p class="text-sm text-slate-400">Active Nodes: <span class="text-white">6/6</span></p>
                    </div>

                     <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">API Gateway</p>
                        <p class="text-3xl font-extrabold text-yellow-500">DEGRADED</p>
                        <p class="text-sm text-slate-400">Egress Bandwidth: <span class="text-white">85%</span></p>
                    </div>

                </div>
            </section>

            <section class="mb-12">
                <h3 class="text-xl font-medium mb-4 border-b border-slate-700 pb-2">🧠 AI Security & Automation Status</h3>
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
                    
                    <div class="card p-5 rounded-lg shadow-xl col-span-2">
                        <p class="text-lg font-bold mb-2">🔐 SynapseAuth (IAM) Risk Report</p>
                        <div class="flex justify-between items-center">
                            <p class="text-4xl font-extrabold ai-status-active">SAFE</p>
                            <p class="text-sm text-slate-400">Highest Risk Score: <span class="ai-status-alert font-bold">45/100</span> (User X)</p>
                        </div>
                        <div class="mt-4">
                            <p class="text-sm text-slate-400">Last Action: <span class="text-white">Blocked 3 attempts from China (Automated)</span></p>
                        </div>
                    </div>

                    <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">🚨 SynapseLogs Alerts</p>
                        <p class="text-3xl font-extrabold ai-status-alert">7 High Alerts</p>
                        <p class="text-sm text-slate-400">Anomaly Detection: <span class="text-white">API Call Volume Spike (300%)</span></p>
                    </div>
                </div>
            </section>

             <section>
                <h3 class="text-xl font-medium mb-4 border-b border-slate-700 pb-2">✨ Huduma za Kivutio & Ufanisi</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    
                    <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">🧾 SynapseAudit (Compliance)</p>
                        <p class="text-3xl font-extrabold text-green-400">100% Compliant</p>
                        <p class="text-sm text-slate-400">Last RTBF Execution: <span class="text-white">Successful (0 errors)</span></p>
                    </div>

                    <div class="card p-5 rounded-lg shadow-xl">
                        <p class="text-lg font-bold mb-2">🔔 SynapseAlerts</p>
                        <p class="text-3xl font-extrabold text-green-400">0 Critical Rules</p>
                        <p class="text-sm text-slate-400">User Alerts Configured: <span class="text-white">14 Rules Active</span></p>
                    </div>

                </div>
            </section>

        </main>
    </div>
</body>
</html>

