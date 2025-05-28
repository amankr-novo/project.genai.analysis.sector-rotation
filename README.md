```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mastering Sector Rotation: Infographic for Indian Retail Investors</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; scroll-behavior: smooth; }
        .chart-container { position: relative; width: 100%; max-width: 600px; margin-left: auto; margin-right: auto; height: 350px; max-height: 450px; }
        @media (max-width: 768px) { .chart-container { height: 300px; max-height: 400px;} }
        .section-title { border-left: 5px solid; padding-left: 10px; }
        .stat-card { transition: transform 0.3s ease, box-shadow 0.3s ease; }
        .stat-card:hover { transform: translateY(-5px); box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1), 0 4px 6px -2px rgba(0,0,0,0.05); }
        .flow-step { border: 2px solid; transition: background-color 0.3s ease, color 0.3s ease; }
        .flow-step:hover { background-color: #FFD166; color: #073B4C; }
        .flow-arrow { font-size: 2rem; line-height: 1; }
        .rrg-quadrant { border: 2px dashed; }
        .sticky-nav { position: -webkit-sticky; position: sticky; top: 0; z-index: 50; }
        .nav-link.active { font-weight: bold; border-bottom: 2px solid; }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- Application Structure Plan: 
        A single, scrollable page with a sticky top navigation for quick jumps. Sections:
        1. Hero: What is Sector Rotation & Why India? (Big text, key stats)
        2. The Economic Engine: Cycles, Sector Behavior (HTML/CSS cycle diagram, Chart.js bar chart for performance)
        3. Strategy Toolkit: Research, Instruments, Timing, Allocation (HTML/CSS flow for top-down, Chart.js radar for instruments)
        4. Smart Investing: Best Practices & Risks (HTML/CSS cards, lists)
        5. Market Pulse: Recent Trends (Mid-2025) (HTML/CSS RRG concept, text summaries)
        6. Conclusion & Empowerment.
        This structure follows the report's flow, adapted for a visually driven infographic experience, making complex information digestible.
    -->
    <!-- Visualization & Content Choices:
        - What is Sector Rotation?: Goal: Inform -> Viz: Large text, simple HTML/CSS diagram (boxes & arrows for "shifting capital"). Justification: Clear, concise definition. Method: HTML/Tailwind.
        - Why Relevant for India?: Goal: Inform -> Viz: "Dynamic Indian Economy" stat card, bullet points for policy/monsoon impact. Justification: Highlight key relevance. Method: HTML/Tailwind.
        - Economic Cycle Phases: Goal: Organize -> Viz: HTML/CSS styled cards in a sequence for 4 phases. Justification: Visually distinct stages. Method: HTML/Tailwind.
        - Sector Performance (Table 1): Goal: Compare -> Viz: Chart.js Grouped Bar Chart (Phases vs. Sector Performance Score). Justification: Clear visual comparison. Library: Chart.js.
        - Macro Indicators (Table 2): Goal: Inform -> Viz: HTML/CSS styled list with icons (Unicode). Justification: Quick, readable info. Method: HTML/Tailwind.
        - Top-Down Approach: Goal: Organize -> Viz: HTML/CSS Flow Diagram (Macro -> Sector -> Stock). Justification: Visual process. Method: HTML/Tailwind.
        - Investment Instruments (Table 4): Goal: Compare -> Viz: Chart.js Radar Chart (Equity vs. MF vs. ETF on Cost, Liquidity, etc.). Justification: Multi-attribute comparison. Library: Chart.js.
        - Best Practices/Risks: Goal: Inform -> Viz: HTML/CSS styled cards/lists. Justification: Digestible chunks of info. Method: HTML/Tailwind.
        - RRG Concept (Recent Trends): Goal: Organize/Inform -> Viz: HTML/CSS 2x2 grid for RRG quadrants with sector labels. Justification: Conceptual visual of RRG. Method: HTML/Tailwind.
        - CONFIRMATION: NO SVG graphics used. NO Mermaid JS used.
    -->

    <nav id="mainNav" class="sticky-nav bg-white shadow-md py-2 px-4 md:px-8">
        <div class="container mx-auto flex flex-wrap justify-center items-center text-sm md:text-base">
            <a href="#intro" class="nav-link text-[#118AB2] hover:text-[#06D6A0] px-3 py-2 rounded-md">Intro</a>
            <a href="#economic-cycle" class="nav-link text-[#118AB2] hover:text-[#06D6A0] px-3 py-2 rounded-md">Economic Cycle</a>
            <a href="#strategy" class="nav-link text-[#118AB2] hover:text-[#06D6A0] px-3 py-2 rounded-md">Strategy</a>
            <a href="#smart-investing" class="nav-link text-[#118AB2] hover:text-[#06D6A0] px-3 py-2 rounded-md">Smart Investing</a>
            <a href="#market-pulse" class="nav-link text-[#118AB2] hover:text-[#06D6A0] px-3 py-2 rounded-md">Market Pulse</a>
            <a href="#conclusion" class="nav-link text-[#118AB2] hover:text-[#06D6A0] px-3 py-2 rounded-md">Conclusion</a>
        </div>
    </nav>

    <div class="container mx-auto p-4 md:p-8 space-y-12 md:space-y-16">

        <section id="intro" class="text-center pt-8">
            <h1 class="text-4xl md:text-5xl font-bold text-[#073B4C] mb-4">Mastering Sector Rotation</h1>
            <p class="text-xl md:text-2xl text-[#118AB2] mb-8">An Indian Retail Investor's Guide to Maximizing Investment Benefits</p>
            
            <div class="grid md:grid-cols-2 gap-8 items-center">
                <div class="bg-white p-6 rounded-lg shadow-lg stat-card border-l-4 border-[#FF6B6B]">
                    <h2 class="text-2xl font-semibold text-[#073B4C] mb-3">What is Sector Rotation?</h2>
                    <p class="text-gray-700 mb-4">An active strategy of shifting investments between economic sectors based on anticipated market and economic cycle changes. The goal: be in the right place at the right time!</p>
                    <div class="flex justify-center items-center space-x-2 text-[#118AB2]">
                        <div class="p-3 bg-blue-100 rounded-md text-sm">Sector A (Current)</div>
                        <span class="text-2xl font-bold text-[#FFD166]">&rarr;</span>
                        <div class="p-3 bg-green-100 rounded-md text-sm">Sector B (Future)</div>
                    </div>
                     <p class="text-xs text-gray-500 mt-3">It's about anticipating, not just reacting.</p>
                </div>

                <div class="bg-white p-6 rounded-lg shadow-lg stat-card border-l-4 border-[#06D6A0]">
                    <h2 class="text-2xl font-semibold text-[#073B4C] mb-3">Why Relevant for India? <span class="text-2xl">🇮🇳</span></h2>
                    <p class="text-gray-700 mb-2">India's dynamic economy sees sectors react swiftly to:</p>
                    <ul class="list-disc list-inside text-left text-gray-600 space-y-1 text-sm">
                        <li>Union Budget & RBI Policies</li>
                        <li>Monsoon Patterns & Rural Demand</li>
                        <li>'Make in India' & Other Govt. Initiatives</li>
                        <li>Global Economic Trends</li>
                    </ul>
                    <p class="text-gray-700 mt-3">Understanding these responses can unlock potential for enhanced returns.</p>
                </div>
            </div>

             <div class="mt-10 grid md:grid-cols-2 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-md stat-card">
                    <h3 class="text-xl font-semibold text-[#06D6A0] mb-2">Benefit 1: Maximize Returns 📈</h3>
                    <p class="text-gray-600 text-sm">Strategically shift to growth-poised sectors to potentially achieve returns superior to the broader market.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md stat-card">
                    <h3 class="text-xl font-semibold text-[#FF6B6B] mb-2">Benefit 2: Manage Risk 🛡️</h3>
                    <p class="text-gray-600 text-sm">Diversify away from underperforming sectors to reduce potential losses and adapt to economic changes.</p>
                </div>
            </div>
        </section>

        <section id="economic-cycle" class="pt-8">
            <h2 class="section-title text-3xl font-bold text-[#073B4C] mb-8 border-[#118AB2]">The Economic Engine: Cycles & Sector Behavior</h2>
            <p class="text-gray-700 mb-6 text-center md:text-left">Understanding the typical phases of an economic cycle is key. India has its own nuances!</p>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
                <div class="bg-white p-6 rounded-lg shadow-lg stat-card border-t-4 border-[#06D6A0]">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-2">1. Recovery / Early Expansion</h3>
                    <p class="text-sm text-gray-600">Economy bottoms out, low interest rates, confidence returns. <strong class="text-[#06D6A0]">Typically Favors:</strong> Auto, Banks, Consumer Discretionary, Real Estate.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg stat-card border-t-4 border-[#FFD166]">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-2">2. Mid-Expansion</h3>
                    <p class="text-sm text-gray-600">Strong GDP growth, rising earnings & investment. <strong class="text-[#FFD166]">Typically Favors:</strong> Industrials, Infrastructure, IT, Capital Goods.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg stat-card border-t-4 border-[#FF6B6B]">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-2">3. Peak</h3>
                    <p class="text-sm text-gray-600">Economy overheats, inflation rises, rate hikes possible. <strong class="text-[#FF6B6B]">Typically Favors:</strong> Metals, Energy, Materials.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg stat-card border-t-4 border-[#118AB2]">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-2">4. Contraction / Slowdown</h3>
                    <p class="text-sm text-gray-600">Declining activity, easing inflation. <strong class="text-[#118AB2]">Typically Favors:</strong> FMCG, Pharma/Healthcare, Utilities, (sometimes IT).</p>
                </div>
            </div>
            
            <div class="bg-white p-6 rounded-lg shadow-lg">
                <h3 class="text-xl font-semibold text-[#073B4C] mb-4 text-center">Typical Indian Sector Performance in Economic Phases</h3>
                <div class="chart-container">
                    <canvas id="sectorPerformanceChart"></canvas>
                </div>
                <p class="text-xs text-gray-500 mt-3 text-center">Illustrative data. Actual performance varies. Source: Guide Table 1.</p>
            </div>

            <div class="mt-8 bg-white p-6 rounded-lg shadow-lg">
                 <h3 class="text-xl font-semibold text-[#073B4C] mb-4">Key Macro Indicators to Watch in India</h3>
                 <ul class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 text-sm">
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#118AB2]">📈</span> GDP Growth</li>
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#FF6B6B]">🔥</span> Inflation (CPI & WPI)</li>
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#06D6A0]">🏦</span> RBI Interest Rates</li>
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#FFD166]">🏭</span> Index of Industrial Production (IIP)</li>
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#118AB2]">💸</span> FII Flows</li>
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#FF6B6B]">🛢️</span> Crude Oil Prices</li>
                    <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#06D6A0]">🔄</span> Rupee Exchange Rate</li>
                     <li class="flex items-center p-3 bg-gray-100 rounded-md"><span class="mr-2 text-[#FFD166]">🌧️</span> Monsoon Performance (Impacts Agri, FMCG, Auto)</li>
                 </ul>
            </div>
        </section>

        <section id="strategy" class="pt-8">
            <h2 class="section-title text-3xl font-bold text-[#073B4C] mb-8 border-[#06D6A0]">The Strategy Toolkit: Research, Instruments & Timing</h2>
            
            <div class="bg-white p-6 rounded-lg shadow-lg mb-8">
                <h3 class="text-xl font-semibold text-[#073B4C] mb-4 text-center">Top-Down Approach to Sector Rotation</h3>
                <div class="flex flex-col md:flex-row justify-around items-center space-y-4 md:space-y-0 md:space-x-4">
                    <div class="flow-step text-center p-4 rounded-lg border-[#118AB2] text-[#118AB2] w-full md:w-1/3">
                        <div class="text-3xl mb-2">🌍</div>
                        <h4 class="font-semibold">1. Analyze Macro Economy</h4>
                        <p class="text-xs">GDP, Inflation, Interest Rates</p>
                    </div>
                    <div class="flow-arrow text-[#FFD166] hidden md:block">&rarr;</div>
                    <div class="flow-arrow text-[#FFD166] md:hidden text-center">&darr;</div>
                    <div class="flow-step text-center p-4 rounded-lg border-[#06D6A0] text-[#06D6A0] w-full md:w-1/3">
                        <div class="text-3xl mb-2">📊</div>
                        <h4 class="font-semibold">2. Identify Promising Sectors</h4>
                        <p class="text-xs">Based on Economic Phase</p>
                    </div>
                    <div class="flow-arrow text-[#FFD166] hidden md:block">&rarr;</div>
                     <div class="flow-arrow text-[#FFD166] md:hidden text-center">&darr;</div>
                    <div class="flow-step text-center p-4 rounded-lg border-[#FF6B6B] text-[#FF6B6B] w-full md:w-1/3">
                        <div class="text-3xl mb-2">💡</div>
                        <h4 class="font-semibold">3. Select Securities</h4>
                        <p class="text-xs">Stocks, ETFs, Mutual Funds</p>
                    </div>
                </div>
            </div>

            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-4">Key Parameters for Sector Analysis</h3>
                    <ul class="list-none space-y-3 text-sm">
                        <li class="p-3 bg-gray-50 rounded-md border-l-2 border-[#118AB2]"><strong class="text-[#118AB2]">Economic Sensitivity:</strong> How sector reacts to changes.</li>
                        <li class="p-3 bg-gray-50 rounded-md border-l-2 border-[#06D6A0]"><strong class="text-[#06D6A0]">Valuation (P/E, P/B):</strong> Over/undervalued vs history/peers.</li>
                        <li class="p-3 bg-gray-50 rounded-md border-l-2 border-[#FFD166]"><strong class="text-[#FFD166]">Growth Drivers:</strong> Tech, policy, demographics.</li>
                        <li class="p-3 bg-gray-50 rounded-md border-l-2 border-[#FF6B6B]"><strong class="text-[#FF6B6B]">Regulatory Environment:</strong> Impending changes.</li>
                        <li class="p-3 bg-gray-50 rounded-md border-l-2 border-[#073B4C]"><strong class="text-[#073B4C]">Relative Strength:</strong> Performance vs market/other sectors.</li>
                    </ul>
                </div>

                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-4 text-center">Choosing Your Investment Instrument</h3>
                    <div class="chart-container">
                        <canvas id="instrumentComparisonChart"></canvas>
                    </div>
                    <p class="text-xs text-gray-500 mt-3 text-center">Illustrative comparison. Source: Guide Table 4.</p>
                </div>
            </div>
            <div class="mt-8 bg-white p-6 rounded-lg shadow-lg">
                <h3 class="text-xl font-semibold text-[#073B4C] mb-4">Timing Your Moves: The Biggest Challenge!</h3>
                <p class="text-gray-700 mb-3 text-sm">Perfect timing is elusive. Consider these:</p>
                <ul class="list-disc list-inside text-gray-600 space-y-1 text-sm">
                    <li>Shifts in economic data & leading indicators.</li>
                    <li>Significant policy announcements (Budget, RBI).</li>
                    <li>Sectoral earnings trends and outlook.</li>
                    <li>Technical signals on sectoral charts (MAs, RSI).</li>
                </ul>
                <p class="mt-3 text-sm text-gray-700"><strong class="text-[#FF6B6B]">Tip:</strong> Consider a gradual, rule-based rotation rather than emotional decisions.</p>
            </div>
        </section>

        <section id="smart-investing" class="pt-8">
            <h2 class="section-title text-3xl font-bold text-[#073B4C] mb-8 border-[#FFD166]">Smart Investing: Best Practices & Key Risks</h2>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-4">Best Practices for Indian Investors</h3>
                    <ul class="list-disc list-inside text-gray-600 space-y-2 text-sm">
                        <li>Adopt a <strong class="text-[#118AB2]">Long-Term Perspective</strong> on underlying trends.</li>
                        <li>Engage in <strong class="text-[#06D6A0]">Continuous Learning</strong> & Monitoring.</li>
                        <li>Manage <strong class="text-[#FF6B6B]">Costs</strong> (Brokerage, STT, Taxes).</li>
                        <li>Mitigate <strong class="text-[#FFD166]">Behavioral Biases</strong> (Herd Mentality, Overconfidence).</li>
                        <li><strong class="text-[#118AB2]">Start Small</strong> if new to the strategy.</li>
                        <li>Align with <strong class="text-[#06D6A0]">Personal Risk Tolerance</strong>.</li>
                        <li>Focus on <strong class="text-[#FF6B6B]">Quality</strong> (companies/ETFs).</li>
                        <li>Maintain an <strong class="text-[#FFD166]">Investment Journal</strong>.</li>
                    </ul>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-lg">
                    <h3 class="text-xl font-semibold text-[#073B4C] mb-4">Key Risks & Challenges</h3>
                     <ul class="list-disc list-inside text-gray-600 space-y-2 text-sm">
                        <li><strong class="text-[#FF6B6B]">Timing Risk:</strong> The biggest hurdle!</li>
                        <li><strong class="text-[#FFD166]">Information Asymmetry:</strong> Retail vs. Institutional.</li>
                        <li><strong class="text-[#06D6A0]">Research Intensity:</strong> Requires time & effort.</li>
                        <li><strong class="text-[#118AB2]">Concentration Risk:</strong> Don't put all eggs in one sector.</li>
                        <li><strong class="text-[#FF6B6B]">Market Volatility</strong> & Sector-Specific Shocks.</li>
                        <li><strong class="text-[#FFD166]">Liquidity Risk:</strong> Especially in niche ETFs/small-caps.</li>
                        <li><strong class="text-[#06D6A0]">Whipsaw Effect:</strong> Caught by false signals.</li>
                        <li><strong class="text-[#118AB2]">Sudden Policy Changes:</strong> A key factor in India.</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="market-pulse" class="pt-8">
            <h2 class="section-title text-3xl font-bold text-[#073B4C] mb-8 border-[#FF6B6B]">Market Pulse: Recent Trends & Expert Opinions (Mid-2025)</h2>
            <p class="text-gray-700 mb-6 text-center md:text-left">Insights based on the report's analysis as of mid-2025. Markets are dynamic!</p>
            <div class="bg-white p-6 rounded-lg shadow-lg mb-8">
                <h3 class="text-xl font-semibold text-[#073B4C] mb-3">Mid-2025 Sectoral Shifts (Conceptual RRG View)</h3>
                <div class="grid grid-cols-2 gap-4 text-center text-sm">
                    <div class="rrg-quadrant p-4 rounded-md border-[#06D6A0] bg-green-50">
                        <h4 class="font-semibold text-[#06D6A0] mb-1">🚀 Leading</h4>
                        <p class="text-gray-600">IT (Improving), Metals (Improving)</p>
                    </div>
                    <div class="rrg-quadrant p-4 rounded-md border-[#FFD166] bg-yellow-50">
                        <h4 class="font-semibold text-[#FFD166] mb-1">📉 Weakening</h4>
                        <p class="text-gray-600">Banking (Waning Strength)</p>
                    </div>
                    <div class="rrg-quadrant p-4 rounded-md border-[#FF6B6B] bg-red-50">
                        <h4 class="font-semibold text-[#FF6B6B] mb-1">🐌 Lagging</h4>
                        <p class="text-gray-600">Pharma, FMCG, Healthcare, Auto (but Auto showing momentum pickup)</p>
                    </div>
                    <div class="rrg-quadrant p-4 rounded-md border-[#118AB2] bg-blue-50">
                        <h4 class="font-semibold text-[#118AB2] mb-1">📈 Improving</h4>
                        <p class="text-gray-600">(Sectors moving from Lagging to Leading - e.g. IT, Metals as per text)</p>
                    </div>
                </div>
                <p class="text-xs text-gray-500 mt-3 text-center">This is a simplified conceptual representation based on report text. Actual RRG is more complex.</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-lg">
                <h3 class="text-xl font-semibold text-[#073B4C] mb-3">Expert Takeaways (Mid-2025)</h3>
                <ul class="list-disc list-inside text-gray-600 space-y-1 text-sm">
                    <li>Watch for emerging leadership from beaten-down sectors showing revival (IT, Metals).</li>
                    <li>Sectors underperforming for 3-5 years could become new leaders (Private Banks, Cement, Oil & Gas, Textiles, Chemicals identified as potential).</li>
                    <li>FY25 Indian economy projected growth: ~6.4-6.5%.</li>
                    <li>Challenges: Sluggish manufacturing, food inflation. Opportunities: Govt. capex, 'China + 1'.</li>
                </ul>
                <p class="mt-3 text-sm text-gray-700 font-semibold">Key: Proactive, forward-looking analysis is crucial.</p>
            </div>
        </section>

        <section id="conclusion" class="text-center py-12 bg-gradient-to-r from-[#118AB2] to-[#06D6A0] rounded-lg shadow-xl mt-8">
            <h2 class="text-3xl md:text-4xl font-bold text-white mb-6">Empower Your Investment Journey!</h2>
            <p class="text-lg text-gray-100 mb-6 mx-auto max-w-3xl">Sector rotation can be a powerful tool for Indian retail investors if approached with diligence, discipline, and a thorough understanding of markets & risks. It's not a "get rich quick" scheme but a strategic approach for long-term wealth creation.</p>
            <p class="text-md text-yellow-300 font-semibold">Continuous learning and informed decision-making are key.</p>
            <p class="text-xs text-gray-200 mt-8">Disclaimer: This infographic is for educational purposes only, based on the provided report. It is not investment advice. Consult a SEBI RIA for personalized guidance.</p>
        </section>

    </div>

    <script>
        function wrapChartLabels(label, maxWidth = 16) {
            const words = label.split(' ');
            let currentLine = '';
            const lines = [];
            for (const word of words) {
                if ((currentLine + word).length > maxWidth && currentLine.length > 0) {
                    lines.push(currentLine.trim());
                    currentLine = word + ' ';
                } else {
                    currentLine += word + ' ';
                }
            }
            if (currentLine.trim().length > 0) {
                lines.push(currentLine.trim());
            }
            return lines.length > 0 ? lines : [label]; 
        }

        const commonTooltipTitleCallback = function(tooltipItems) {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
                return label.join(' ');
            }
            return label;
        };
        
        const commonChartOptions = {
            responsive: true,
            maintainAspectRatio: false,
            plugins: {
                legend: {
                    labels: { color: '#073B4C' }
                },
                tooltip: {
                    callbacks: { title: commonTooltipTitleCallback },
                    backgroundColor: '#073B4C',
                    titleColor: '#FFD166',
                    bodyColor: '#FFFFFF',
                }
            },
            scales: {
                y: {
                    beginAtZero: true,
                    grid: { color: 'rgba(7,59,76,0.1)' },
                    ticks: { color: '#073B4C' }
                },
                x: {
                    grid: { display: false },
                    ticks: { 
                        color: '#073B4C',
                        callback: function(value, index, ticks) {
                            const label = this.getLabelForValue(value);
                            return wrapChartLabels(label);
                        }
                    }
                }
            }
        };

        const sectorPerformanceData = {
            labels: ['Recovery/ Early Expansion', 'Mid-Expansion', 'Peak', 'Contraction/ Slowdown'],
            datasets: [
                {
                    label: 'Auto & Real Estate',
                    data: [7, 6, 3, 2],
                    backgroundColor: '#FF6B6B',
                    borderColor: '#E55A5A',
                    borderWidth: 1
                },
                {
                    label: 'Banks & Financials',
                    data: [8, 7, 4, 3],
                    backgroundColor: '#FFD166',
                    borderColor: '#E5B95A',
                    borderWidth: 1
                },
                {
                    label: 'IT & Industrials',
                    data: [6, 8, 6, 5],
                    backgroundColor: '#06D6A0',
                    borderColor: '#05BFA0',
                    borderWidth: 1
                },
                {
                    label: 'FMCG & Pharma (Defensive)',
                    data: [4, 5, 7, 8],
                    backgroundColor: '#118AB2',
                    borderColor: '#0F79A1',
                    borderWidth: 1
                }
            ]
        };
        new Chart(document.getElementById('sectorPerformanceChart'), {
            type: 'bar',
            data: sectorPerformanceData,
            options: { ...commonChartOptions, plugins: { ...commonChartOptions.plugins, title: { display: true, text: 'Illustrative Sector Performance Scores', color: '#073B4C', font: {size: 14} } } }
        });

        const instrumentData = {
            labels: wrapChartLabels('Cost Effectiveness (Lower is Better)', 12).concat(
                wrapChartLabels('Liquidity (Higher is Better)', 12),
                wrapChartLabels('Diversification (Higher is Better)', 12),
                wrapChartLabels('Research Burden (Lower is Better)', 12),
                wrapChartLabels('Trading Flexibility (Higher is Better)', 12)
            ),
            datasets: [{
                label: 'Direct Equity',
                data: [2, 3, 1, 1, 5], // Cost: Higher(2), Liquidity: Varies(3), Diversification: Low(1), Research: High(1), Flex: High(5)
                borderColor: '#FF6B6B',
                backgroundColor: 'rgba(255, 107, 107, 0.2)',
                pointBackgroundColor: '#FF6B6B',
                pointBorderColor: '#fff',
                pointHoverBackgroundColor: '#fff',
                pointHoverBorderColor: '#FF6B6B'
            }, {
                label: 'Sectoral MFs',
                data: [3, 4, 4, 4, 2], // Cost: Mid-High(3), Liquidity: Good(4), Diversification: High(4), Research: Low(4), Flex: Low(2)
                borderColor: '#FFD166',
                backgroundColor: 'rgba(255, 209, 102, 0.2)',
                pointBackgroundColor: '#FFD166',
                pointBorderColor: '#fff',
                pointHoverBackgroundColor: '#fff',
                pointHoverBorderColor: '#FFD166'
            }, {
                label: 'Sectoral ETFs',
                data: [4, 3.5, 4, 3, 5], // Cost: Low(4), Liquidity: Varies(3.5), Diversification: High(4), Research: Mid(3), Flex: High(5)
                borderColor: '#06D6A0',
                backgroundColor: 'rgba(6, 214, 160, 0.2)',
                pointBackgroundColor: '#06D6A0',
                pointBorderColor: '#fff',
                pointHoverBackgroundColor: '#fff',
                pointHoverBorderColor: '#06D6A0'
            }]
        };
        new Chart(document.getElementById('instrumentComparisonChart'), {
            type: 'radar',
            data: instrumentData,
            options: {
                responsive: true,
                maintainAspectRatio: false,
                elements: { line: { borderWidth: 2 } },
                scales: {
                    r: {
                        angleLines: { display: true, color: 'rgba(7,59,76,0.2)' },
                        suggestedMin: 0,
                        suggestedMax: 5,
                        grid: { color: 'rgba(7,59,76,0.2)' },
                        pointLabels: { 
                            font: { size: 10 }, 
                            color: '#073B4C',
                            callback: function(labelArray) { return labelArray; } // Already an array
                        },
                        ticks: { 
                            display: true, 
                            stepSize: 1, 
                            backdropColor: 'rgba(255,255,255,0.75)', 
                            color: '#118AB2',
                            font: {weight: 'bold'}
                        }
                    }
                },
                plugins: {
                    legend: { position: 'top', labels: { color: '#073B4C'} },
                    title: { display: true, text: 'Investment Instruments (Scores 1-5)', color: '#073B4C', font: {size: 14} },
                    tooltip: {
                        callbacks: {
                             title: function(tooltipItems) { // Custom title for radar
                                return tooltipItems[0].dataset.label;
                             },
                             label: function(tooltipItem) {
                                let label = tooltipItem.chart.data.labels[tooltipItem.dataIndex];
                                if(Array.isArray(label)) label = label.join(' ');
                                return `${label}: ${tooltipItem.formattedValue}`;
                             }
                        },
                        backgroundColor: '#073B4C',
                        titleColor: '#FFD166',
                        bodyColor: '#FFFFFF',
                    }
                }
            }
        });

        // Sticky Nav Active Link Highlighting
        const navLinks = document.querySelectorAll('.nav-link');
        const sections = document.querySelectorAll('section[id]');

        function changeNav() {
            let index = sections.length;
            while(--index && window.scrollY + 100 < sections[index].offsetTop) {}
            
            navLinks.forEach((link) => link.classList.remove('active', 'border-[#06D6A0]', 'text-[#06D6A0]'));
            if (sections[index]) { // Check if sections[index] exists
                 const activeLink = document.querySelector(`.nav-link[href="#${sections[index].id}"]`);
                 if (activeLink) {
                    activeLink.classList.add('active', 'border-[#06D6A0]', 'text-[#06D6A0]');
                 }
            }
        }
        changeNav(); // Initial call
        window.addEventListener('scroll', changeNav);

    </script>
</body>
</html>

```
