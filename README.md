<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infográfico: Navegando pela Nova Experiência do Usuário</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .chart-container {
            position: relative;
            width: 100%;
            height: 320px;
            max-height: 400px;
        }
        @media (min-width: 640px) {
            .chart-container {
                height: 380px;
            }
        }
        .flowchart-item {
            position: relative;
            z-index: 1;
        }
        .flowchart-item:not(:last-child)::after {
            content: '▼';
            position: absolute;
            bottom: -28px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 24px;
            color: #94D2BD;
            z-index: 0;
        }
        .timeline {
            position: relative;
            padding: 2rem 0;
        }
        .timeline::before {
            content: '';
            position: absolute;
            top: 0;
            left: 18px;
            height: 100%;
            width: 4px;
            background: #94D2BD;
            border-radius: 2px;
        }
        .timeline-item {
            position: relative;
            padding-left: 4rem;
            margin-bottom: 2rem;
        }
        .timeline-item::before {
            content: '';
            position: absolute;
            left: 10px;
            top: 5px;
            height: 20px;
            width: 20px;
            border-radius: 50%;
            background: #0A9396;
            border: 3px solid #94D2BD;
        }
    </style>
</head>
<body class="bg-[#001219] text-gray-200">

    <div class="max-w-7xl mx-auto p-4 sm:p-6 lg:p-8">
        
        <header class="text-center mb-16">
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">Navegando pela Nova Experiência do Usuário</h1>
            <p class="text-lg text-[#94D2BD]">Uma interface mais inteligente para decisões mais rápidas e gestão eficiente.</p>
        </header>

        <main class="grid grid-cols-1 md:grid-cols-2 gap-8">

            <section class="md:col-span-2 bg-[#005F73] rounded-lg shadow-2xl p-6">
                <h2 class="text-2xl font-bold text-white mb-4 text-center">Jornada do Usuário Simplificada</h2>
                <p class="text-center text-[#94D2BD] mb-8">O novo fluxo permite que os usuários, de gerentes a analistas, acessem e interajam com os dados de forma mais intuitiva e direta.</p>
                <div class="flex flex-col md:flex-row justify-around items-center space-y-8 md:space-y-0 md:space-x-4">
                    <div class="flowchart-item text-center">
                        <div class="bg-[#0A9396] rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-2 shadow-lg">
                            <span class="text-4xl">🔑</span>
                        </div>
                        <h3 class="font-semibold text-white">1. Login e Dashboard</h3>
                        <p class="text-xs text-[#94D2BD]">Visão geral imediata</p>
                    </div>
                    <div class="flowchart-item text-center">
                        <div class="bg-[#0A9396] rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-2 shadow-lg">
                            <span class="text-4xl">📊</span>
                        </div>
                        <h3 class="font-semibold text-white">2. Análise de Tabelas</h3>
                        <p class="text-xs text-[#94D2BD]">Projetos e Finanças</p>
                    </div>
                    <div class="flowchart-item text-center">
                        <div class="bg-[#0A9396] rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-2 shadow-lg">
                            <span class="text-4xl">🔍</span>
                        </div>
                        <h3 class="font-semibold text-white">3. Detalhes do Projeto</h3>
                        <p class="text-xs text-[#94D2BD]">Histórico e Status</p>
                    </div>
                    <div class="flowchart-item text-center">
                        <div class="bg-[#0A9396] rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-2 shadow-lg">
                            <span class="text-4xl">🛠️</span>
                        </div>
                        <h3 class="font-semibold text-white">4. Logs de Auditoria</h3>
                        <p class="text-xs text-[#94D2BD]">Depuração e Segurança</p>
                    </div>
                </div>
            </section>

            <section class="bg-white rounded-lg shadow-lg p-6 text-[#001219]">
                <h2 class="text-2xl font-bold mb-4">Clareza Instantânea com Status Visual</h2>
                <p class="mb-6">Identifique rapidamente o estado de cada projeto com um sistema de cores intuitivo. Menos tempo lendo, mais tempo agindo.</p>
                <ul class="space-y-2">
                    <li class="flex items-center"><span class="h-4 w-4 rounded-full bg-green-500 mr-3"></span>Ativo / Concluído</li>
                    <li class="flex items-center"><span class="h-4 w-4 rounded-full bg-yellow-400 mr-3"></span>Em Andamento</li>
                    <li class="flex items-center"><span class="h-4 w-4 rounded-full bg-orange-500 mr-3"></span>Suspenso</li>
                    <li class="flex items-center"><span class="h-4 w-4 rounded-full bg-red-600 mr-3"></span>Encerrado / Cancelado</li>
                </ul>
                <div class="mt-6">
                    <p class="font-semibold mb-2">Visão do Portfólio:</p>
                    <div class="flex space-x-2 text-3xl">
                        <span class="text-green-500">●</span>
                        <span class="text-green-500">●</span>
                        <span class="text-yellow-400">●</span>
                        <span class="text-yellow-400">●</span>
                        <span class="text-yellow-400">●</span>
                        <span class="text-orange-500">●</span>
                        <span class="text-red-600">●</span>
                    </div>
                </div>
            </section>

            <section class="bg-white rounded-lg shadow-lg p-6 text-[#001219]">
                <h2 class="text-2xl font-bold mb-4">Distribuição de Projetos por Status</h2>
                <p class="mb-6">Visualize a composição do seu portfólio de projetos. A funcionalidade de filtro permite focar em categorias específicas para uma análise aprofundada.</p>
                <div class="chart-container mx-auto max-w-sm">
                    <canvas id="projectStatusChart"></canvas>
                </div>
            </section>

            <section class="md:col-span-2 bg-white rounded-lg shadow-lg p-6 text-[#001219]">
                <h2 class="text-2xl font-bold mb-4 text-center">Domine Seus Dados: Filtro e Ordenação</h2>
                <p class="text-center mb-8">Novas ferramentas poderosas permitem que você organize e encontre as informações que precisa em segundos, tanto em tabelas de projetos quanto em lançamentos financeiros.</p>
                <div class="flex flex-col md:flex-row justify-around items-start space-y-8 md:space-y-0">
                    <div class="text-center w-full md:w-1/2">
                        <h3 class="font-semibold text-lg mb-4">Ordenação com um Clique</h3>
                        <div class="bg-gray-100 rounded-lg p-4 shadow-inner">
                            <div class="flex justify-between items-center bg-gray-200 p-2 rounded-t-lg font-bold">
                                <span>Nome do Projeto ↑</span>
                                <span>Status</span>
                                <span>Orçamento</span>
                            </div>
                            <div class="p-2">Clique nos cabeçalhos para ordenar.</div>
                        </div>
                    </div>
                    <div class="text-center w-full md:w-1/2">
                        <h3 class="font-semibold text-lg mb-4">Filtragem Inteligente</h3>
                         <div class="bg-gray-100 rounded-lg p-4 shadow-inner space-y-3">
                            <input type="text" placeholder="Buscar por nome..." class="w-full p-2 rounded border">
                            <select class="w-full p-2 rounded border">
                                <option>Filtrar por Status</option>
                                <option>Ativo</option>
                                <option>Suspenso</option>
                            </select>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="bg-white rounded-lg shadow-lg p-6 text-[#001219]">
                <h2 class="text-2xl font-bold mb-4">Histórico Transparente do Projeto</h2>
                <p class="mb-6">Acesse um registro cronológico de todas as suspensões de um projeto. Entenda os desafios passados para planejar um futuro de sucesso.</p>
                <div class="timeline">
                    <div class="timeline-item">
                        <h4 class="font-bold text-lg">Projeto Iniciado</h4>
                        <p class="text-sm text-gray-500">15 de Janeiro, 2024</p>
                    </div>
                    <div class="timeline-item">
                        <h4 class="font-bold text-lg text-[#EE9B00]">Projeto Suspenso</h4>
                        <p class="text-sm text-gray-500">20 de Março, 2024</p>
                        <p class="mt-1">Motivo: Reavaliação de escopo pela diretoria.</p>
                    </div>
                    <div class="timeline-item">
                        <h4 class="font-bold text-lg text-green-600">Projeto Retomado</h4>
                        <p class="text-sm text-gray-500">05 de Abril, 2024</p>
                    </div>
                     <div class="timeline-item">
                        <h4 class="font-bold text-lg">Entrega da Fase 1</h4>
                        <p class="text-sm text-gray-500">30 de Maio, 2024</p>
                    </div>
                </div>
            </section>
            
            <section class="bg-white rounded-lg shadow-lg p-6 text-[#001219]">
                <h2 class="text-2xl font-bold mb-4">Rastreabilidade e Segurança</h2>
                <p class="mb-6">O novo sistema de logging registra ações críticas, oferecendo uma camada extra de segurança, auditoria e facilitando a depuração de problemas.</p>
                <div class="chart-container mx-auto">
                    <canvas id="systemActionsChart"></canvas>
                </div>
            </section>

        </main>

        <footer class="text-center mt-16 pt-8 border-t border-[#005F73]">
            <p class="text-[#94D2BD]">&copy; 2025 Infográfico de Melhorias do Sistema. Todos os direitos reservados.</p>
        </footer>

    </div>

    <script>
        function wrapLabel(label, maxWidth) {
            const words = label.split(' ');
            const lines = [];
            let currentLine = '';
            for (const word of words) {
                if ((currentLine + ' ' + word).length > maxWidth && currentLine.length > 0) {
                    lines.push(currentLine);
                    currentLine = word;
                } else {
                    currentLine = currentLine.length === 0 ? word : currentLine + ' ' + word;
                }
            }
            lines.push(currentLine);
            return lines;
        }
        
        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
                return label.join(' ');
            }
            return label;
        };
        
        const sharedTooltipOptions = {
            plugins: {
                tooltip: {
                    callbacks: {
                        title: tooltipTitleCallback
                    }
                }
            }
        };

        const projectStatusCtx = document.getElementById('projectStatusChart').getContext('2d');
        new Chart(projectStatusCtx, {
            type: 'doughnut',
            data: {
                labels: ['Ativo', 'Em Andamento', 'Suspenso', 'Concluído', 'Cancelado'],
                datasets: [{
                    label: 'Projetos por Status',
                    data: [35, 25, 10, 20, 10],
                    backgroundColor: [
                        '#22c55e', // green-500
                        '#f59e0b', // yellow-500
                        '#f97316', // orange-500
                        '#3b82f6', // blue-500
                        '#ef4444'  // red-500
                    ],
                    borderColor: '#ffffff',
                    borderWidth: 3
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            color: '#001219'
                        }
                    },
                    tooltip: sharedTooltipOptions.plugins.tooltip
                }
            }
        });

        const systemActionsCtx = document.getElementById('systemActionsChart').getContext('2d');
        new Chart(systemActionsCtx, {
            type: 'bar',
            data: {
                labels: ['Seg', 'Ter', 'Qua', 'Qui', 'Sex'].map(l => wrapLabel(l, 16)),
                datasets: [
                    {
                        label: 'Atualização de Projeto',
                        data: [12, 19, 15, 22, 18],
                        backgroundColor: '#0A9396',
                    },
                    {
                        label: 'Lançamento Financeiro',
                        data: [30, 25, 40, 33, 38],
                        backgroundColor: '#94D2BD',
                    },
                    {
                        label: 'Mudança de Status',
                        data: [5, 8, 3, 6, 4],
                        backgroundColor: '#EE9B00',
                    }
                ]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    x: {
                        stacked: true,
                        ticks: { color: '#001219' },
                        grid: { display: false }
                    },
                    y: {
                        stacked: true,
                        beginAtZero: true,
                        ticks: { color: '#001219' },
                        grid: { color: '#e5e7eb' }
                    }
                },
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            color: '#001219'
                        }
                    },
                    tooltip: {
                        ...sharedTooltipOptions.plugins.tooltip,
                        mode: 'index',
                        intersect: false
                    }
                }
            }
        });
    </script>
</body>
</html>
