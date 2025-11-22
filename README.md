<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>J-Genki 個人報告書 - TRẦN VÕ THANH THẢO</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Noto+Sans+JP:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', 'Noto Sans JP', sans-serif;
            background-color: #f4f7f6;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 900px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
        }
        .chart-container-small {
            position: relative;
            width: 100%;
            max-width: 350px;
            margin-left: auto;
            margin-right: auto;
            height: 250px;
            max-height: 300px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
            .chart-container-small {
                height: 300px;
            }
        }
        .card {
            background-color: #ffffff;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
            padding: 1.5rem;
            transition: all 0.3s ease;
        }
        .card:hover {
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        .accent-bg {
            background-color: #118AB2;
        }
        .accent-text {
            color: #118AB2;
        }
        .success-bg {
            background-color: #06D6A0;
        }
        .success-text {
            color: #06D6A0;
        }
        .warn-bg {
            background-color: #FFD166;
        }
        .warn-text {
            color: #FFD166;
        }
        .danger-bg {
            background-color: #FF6B6B;
        }
        .danger-text {
            color: #FF6B6B;
        }
        .dark-text {
            color: #073B4C;
        }
    </style>
</head>
<body class="text-gray-800">

    <main class="container mx-auto p-4 md:p-8 max-w-7xl">

        <header class="text-center mb-12">
            <h1 class="text-4xl md:text-5xl font-bold dark-text mb-2">J-Genki 個人報告書</h1>
            <p class="text-xl md:text-2xl accent-text font-semibold">TRẦN VÕ THANH THẢOの8週間の結果</p>
        </header>

        <section id="goals" class="mb-12">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="card">
                    <h2 class="text-2xl font-bold accent-text mb-4">私の目標：ウォーキング</h2>
                    <p class="text-lg mb-4">J-Genkiプログラムでの私の目標は、1日の平均歩数を6,000歩にすることでした。また、エレベーターの代わりに階段を使ったり、学校や家の周りを歩いたりして、積極的に歩数を増やすよう頑張りました。</p>
                    <div class="text-center">
                        <span class="text-6xl font-bold accent-text">6,000</span>
                        <span class="text-xl dark-text ml-2">歩/日 (目標)</span>
                    </div>
                </div>
                <div class="card">
                    <h2 class="text-2xl font-bold success-text mb-4">私の目標：健康的な食生活</h2>
                    <p class="text-lg mb-4">もう一つの目標は、栄養バランスが良くて、しかもおいしい料理を作れるようになることです。この8週間、私は、たんぱく質、食物繊維、炭水化物、果物を食べるように心がけました。</p>
                    <div class="text-center">
                        <span class="text-5xl success-text">🥗 🍜 🍚</span>
                        <p class="text-xl dark-text mt-2">バランスの良い自炊</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="walking-challenge" class="card mb-12">
            <h2 class="text-3xl font-bold dark-text text-center mb-2">ウォーキングチャレンジの結果</h2>
            <p class="text-lg text-gray-600 text-center mb-8">8週間の平均歩数の推移です。目標の6,000歩ライン（赤）を常に上回ることができましたが、第7週は試験勉強で一時的に減少しました。</p>
            <div class="chart-container">
                <canvas id="stepsChart"></canvas>
            </div>
            <div class="text-center mt-8 p-6 bg-blue-50 rounded-lg">
                <p class="text-xl dark-text">8週間の総平均</p>
                <p class="text-6xl font-bold accent-text my-2">8,126</p>
                <p class="text-2xl success-text font-semibold">目標を 35% 以上達成！</p>
            </div>
        </section>

        <section id="weekly-highlights" class="mb-12">
            <h2 class="text-3xl font-bold dark-text text-center mb-8">毎週の活動ハイライト</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                
                <div class="card">
                    <span class="text-sm font-semibold accent-text">第1週</span>
                    <p class="text-lg font-bold dark-text mt-1">動物園でスタート</p>
                    <p class="text-gray-600">友人と動植物園を散策して、リラックスしながらエネルギーを充電できました。忙しかったたけど、健康的な食べ物を選びました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">9,706 歩</p>
                </div>
                
                <div class="card">
                    <span class="text-sm font-semibold accent-text">第2週</span>
                    <p class="text-lg font-bold dark-text mt-1">旅行とトレーニングの両立</p>
                    <p class="text-gray-600">ブンタウへ旅行して、バックビーチを散歩したり、タムタンタワーを見学しました。旅行中も歩く習慣を維持しました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">7,722 歩</p>
                </div>

                <div class="card">
                    <span class="text-sm font-semibold accent-text">第3週</span>
                    <p class="text-lg font-bold dark-text mt-1">多忙な活動と自炊への挑戦</p>
                    <p class="text-gray-600">中秋節イベントや大学の「Open day」など様々な活動をしました。忙しかったですが、難しい料理も作れるようになりました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">7,867 歩</p>
                </div>

                <div class="card">
                    <span class="text-sm font-semibold accent-text">第4週</span>
                    <p class="text-lg font-bold dark-text mt-1">学業後の散策とお寺</p>
                    <p class="text-gray-600">授業の後、「ファップホア寺院」を訪問しました。静かな散歩でストレスからリラックスして、J-Genkiレシピでサラダを初めて作りました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">7,395 歩</p>
                </div>

                <div class="card">
                    <span class="text-sm font-semibold accent-text">第5週</span>
                    <p class="text-lg font-bold dark-text mt-1">ショッピングモールでの有効活用</p>
                    <p class="text-gray-600">ヴァンハンモールでショッピングとウォーキングを兼ねて、空き時間にはキャンパス内を歩いて時間を有効活用しました。新しいサラダも作りました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">8,596 歩</p>
                </div>

                <div class="card">
                    <span class="text-sm font-semibold accent-text">第6週</span>
                    <p class="text-lg font-bold dark-text mt-1">歴史学習と家族の味</p>
                    <p class="text-gray-600">戦争証跡博物館へ行って、歩きながら歴史も勉強しました。母と一緒にブンボーフエを作って、素敵な思い出になりました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">8,512 歩</p>
                </div>

                <div class="card border-2 border-yellow-300">
                    <span class="text-sm font-semibold warn-text">第7週</span>
                    <p class="text-lg font-bold dark-text mt-1">試練の中間試験</p>
                    <p class="text-gray-600">試験と悪天候で歩数が減少しました。しかし、諦めず夜の公園や室内で歩行を維持しました。母からコムタムの作り方を教わりました。</p>
                    <p class="text-xl font-bold warn-text text-right mt-2">6,852 歩</p>
                </div>

                <div class="card">
                    <span class="text-sm font-semibold accent-text">最終第8週</span>
                    <p class="text-lg font-bold dark-text mt-1">街歩きと家族との時間</p>
                    <p class="text-gray-600">グエンフエ通りを散歩して、その際、ホーチミン市のノートルダム大聖堂を眺めたり、クリスマス前の雰囲気を楽しんだりしました*。母との買い物でも良い思い出を作りました。</p>
                    <p class="text-xl font-bold accent-text text-right mt-2">7,037 歩</p>
                </div>

            </div>
        </section>

        <section id="eating-challenge" class="card mb-12">
            <h2 class="text-3xl font-bold dark-text text-center mb-8">食生活チャレンジの変遷</h2>
            <p class="text-lg text-gray-600 text-center mb-8">忙しい外食中心から、栄養バランスを考えた自炊中心の生活へと移行しました。</p>
            
            <div class="flex flex-col md:flex-row items-center justify-around">
                <div class="text-center p-6">
                    <h3 class="text-2xl font-bold dark-text mb-4">BEFORE</h3>
                    <p class="text-5xl mb-4">🛒</p>
                    <p class="text-lg text-gray-600">忙しくて外食が多い</p>
                    <p class="text-lg text-gray-600">栄養バランスが偏りがち</p>
                </div>

                <div class="text-6xl accent-text my-8 md:my-0">
                    →
                </div>
                
                <div class="text-center p-6">
                    <h3 class="text-2xl font-bold success-text mb-4">AFTER</h3>
                    <p class="text-5xl mb-4">👩‍🍳</p>
                    <p class="text-lg text-gray-600">自炊で栄養を管理</p>
                    <p class="text-lg text-gray-600">新しいレシピに挑戦</p>
                </div>
            </div>

            <div class="mt-8">
                <h4 class="text-xl font-semibold dark-text text-center mb-4">挑戦した主な健康メニュー</h4>
                <div class="flex flex-wrap justify-center gap-4">
                    <span class="text-lg font-medium success-bg text-white px-4 py-2 rounded-full">🥗 J-Genkiのサラダ</span>
                    <span class="text-lg font-medium success-bg text-white px-4 py-2 rounded-full">🍚 ビビンバ (Cơm trộn)</span>
                    <span class="text-lg font-medium success-bg text-white px-4 py-2 rounded-full">🍜 ブンボーフエ (Bún Bò Huế)</span>
                    <span class="text-lg font-medium success-bg text-white px-4 py-2 rounded-full">🍚 コムタム (Cơm Tấm)</span>
                </div>
            </div>
        </section>

        <section id="results" class="mb-12">
            <h2 class="text-3xl font-bold dark-text text-center mb-8">8週間後の成果と感想</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="card flex flex-col items-center justify-center">
                    <h3 class="text-2xl font-bold dark-text mb-4">歩数目標：大幅達成</h3>
                    <div class="chart-container-small">
                        <canvas id="goalChart"></canvas>
                    </div>
                    <p class="text-lg text-gray-600 text-center mt-4">目標の6,000歩に対して、平均で2,126歩も多く歩くことができました。</p>
                </div>
                <div class="card">
                    <h3 class="text-2xl font-bold dark-text mb-4">得られた成果</h3>
                    <ul class="space-y-4">
                        <li class="flex items-start">
                            <span class="text-2xl success-text mr-3">✔</span>
                            <p class="text-lg text-gray-700">体力の向上:　長時間歩いても疲れにくくなって、より活動的になりました。</p>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl success-text mr-3">✔</span>
                            <p class="text-lg text-gray-700">自炊スキルの向上: 伝統的なベトナム料理にも挑戦して、料理への自信がつきました。</p>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl success-text mr-3">✔</span>
                            <p class="text-lg text-gray-700">集中力の向上: バランスの取れた食生活が、学業の集中力維持にも繋がりました。</p>
                        </li>
                        <li class="flex items-start">
                            <span class="text-2xl success-text mr-3">✔</span>
                            <p class="text-lg text-gray-700">ポジティブな習慣の定着: 健康的な生活が「義務」ではなく「楽しみ」の一部となりました。</p>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <footer class="card text-center">
            <h3 class="text-2xl font-bold accent-text mb-4">プログラムを終えて</h3>
            <p class="text-lg text-gray-700 max-w-3xl mx-auto">J-Genkiプログラムは、単なる健康増進ではなくて、私自身の「生活と街を探求する旅」でした。忙しい中でも時間をやりくりして、目標を達成しようと努力した経験は、私に規律と柔軟性を与えてくれました。この8週間で得られたポジティブな習慣と貴重な経験に、心から感謝しています。</p>
        </footer>

    </main>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const chartColors = {
                primary: '#118AB2',
                primaryLight: 'rgba(17, 138, 178, 0.1)',
                success: '#06D6A0',
                warning: '#FFD166',
                danger: '#FF6B6B',
                dark: '#073B4C',
                grid: 'rgba(7, 59, 76, 0.1)'
            };

            const defaultTooltipCallback = {
                title: function(tooltipItems) {
                    const item = tooltipItems[0];
                    let label = item.chart.data.labels[item.dataIndex];
                    if (Array.isArray(label)) {
                        return label.join(' ');
                    } else {
                        return label;
                    }
                }
            };

            if (document.getElementById('stepsChart')) {
                const ctxSteps = document.getElementById('stepsChart').getContext('2d');
                new Chart(ctxSteps, {
                    type: 'line',
                    data: {
                        labels: ['第1週', '第2週', '第3週', '第4週', '第5週', '第6週', '第7週', '第8週'],
                        datasets: [
                            {
                                label: '平均歩数',
                                data: [9706, 7722, 7867, 7395, 8596, 8512, 6852, 7037],
                                borderColor: chartColors.primary,
                                backgroundColor: chartColors.primaryLight,
                                fill: true,
                                tension: 0.3,
                                borderWidth: 3
                            },
                            {
                                label: '目標',
                                data: [6000, 6000, 6000, 6000, 6000, 6000, 6000, 6000],
                                borderColor: chartColors.danger,
                                borderDash: [5, 5],
                                fill: false,
                                borderWidth: 2,
                                pointRadius: 0
                            }
                        ]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        scales: {
                            y: {
                                beginAtZero: false,
                                suggestedMin: 5000,
                                ticks: {
                                    color: chartColors.dark,
                                    font: { weight: '600' }
                                },
                                grid: {
                                    color: chartColors.grid
                                }
                            },
                            x: {
                                ticks: {
                                    color: chartColors.dark,
                                    font: { weight: '600' }
                                },
                                grid: {
                                    display: false
                                }
                            }
                        },
                        plugins: {
                            legend: {
                                position: 'top',
                                labels: {
                                    color: chartColors.dark,
                                    font: { size: 14 }
                                }
                            },
                            tooltip: {
                                callbacks: defaultTooltipCallback
                            }
                        }
                    }
                });
            }

            if (document.getElementById('goalChart')) {
                const ctxGoal = document.getElementById('goalChart').getContext('2d');
                new Chart(ctxGoal, {
                    type: 'doughnut',
                    data: {
                        labels: [
                            ['達成した目標歩数', '(Goal Met)'],
                            '追加の歩数 (Bonus Steps)'
                        ],
                        datasets: [{
                            data: [6000, 2126],
                            backgroundColor: [
                                chartColors.success,
                                chartColors.primary
                            ],
                            hoverBackgroundColor: [
                                '#05b087',
                                '#0f7ca0'
                            ],
                            borderColor: '#ffffff',
                            borderWidth: 4
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        cutout: '70%',
                        plugins: {
                            legend: {
                                position: 'bottom',
                                labels: {
                                    color: chartColors.dark,
                                    font: { size: 12 },
                                    padding: 15,
                                    boxWidth: 12,
                                    usePointStyle: true
                                }
                            },
                            tooltip: {
                                callbacks: defaultTooltipCallback
                            }
                        }
                    }
                });
            }
        });
    </script>
</body>
</html>
