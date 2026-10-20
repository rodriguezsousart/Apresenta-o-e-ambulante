<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-Ambulante - Apresentação Institucional</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            -webkit-tap-highlight-color: transparent;
        }
        .slide-card {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .text-gradient {
            background: linear-gradient(135deg, #059669 0%, #d97706 50%, #ea580c 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
    </style>
</head>
<body class="bg-slate-900 text-slate-100 min-h-screen flex flex-col justify-between selection:bg-emerald-500 selection:text-white">

    <!-- Header Fixo Mobile -->
    <header class="sticky top-0 z-50 bg-slate-900/90 backdrop-blur-md border-b border-slate-800 px-4 py-3 flex items-center justify-between">
        <div class="flex items-center gap-3">
            <img src="https://lh3.googleusercontent.com/gg-dl/AHiVA1kMpPlDEEz8HIqjYg-pJ8PiSYxWX-2N0d3rACajcyBIHdAecPl1GUkOtHXelGeUD00KiErheuHr1kC-xQu_LMSpW8caGivXfoo7oEI7LdV-_IgOYuiNP_02inN5UMbsLhPQ_KTketP6yLGbETWd9T-vK5LhbHqrLdxVmSyFIpEVaJR61Q" alt="Logo E-Ambulante" class="w-8 h-8 rounded-lg shadow-md object-cover">
            <div>
                <h1 class="text-xs font-bold tracking-wider text-slate-200 uppercase">E-Ambulante</h1>
                <p class="text-[10px] text-emerald-400 font-medium">Apresentação Institucional</p>
            </div>
        </div>

        <!-- Controles de Leitura e Tema -->
        <div class="flex items-center gap-2">
            <button id="themeToggle" onclick="toggleTheme()" class="p-2 text-slate-400 hover:text-white bg-slate-800 rounded-lg text-xs flex items-center gap-1 border border-slate-700">
                <i class="fa-solid fa-sun" id="themeIcon"></i>
                <span id="themeLabel" class="hidden sm:inline text-[11px]">Modo Claro</span>
            </button>
            <div class="flex bg-slate-800 rounded-lg p-1 border border-slate-700">
                <button onclick="adjustFontSize(-1)" class="w-7 h-7 flex items-center justify-center text-slate-300 hover:text-white text-xs font-bold">-A</button>
                <button onclick="adjustFontSize(1)" class="w-7 h-7 flex items-center justify-center text-slate-300 hover:text-white text-xs font-bold">+A</button>
            </div>
        </div>
    </header>

    <!-- Indicador de Progresso (Barra) -->
    <div class="w-full bg-slate-800 h-1">
        <div id="progressBar" class="bg-gradient-to-r from-emerald-500 via-amber-500 to-orange-500 h-1 w-1/11 transition-all duration-300"></div>
    </div>

    <!-- Conteúdo Principal do Slide -->
    <main class="flex-1 max-w-2xl w-full mx-auto p-4 sm:p-6 flex flex-col justify-center my-auto">
        
        <!-- Slide 1 -->
        <div class="slide-card space-y-6" id="slide-1">
            <div class="text-center space-y-4 py-6">
                <img src="https://lh3.googleusercontent.com/gg-dl/AHiVA1kMpPlDEEz8HIqjYg-pJ8PiSYxWX-2N0d3rACajcyBIHdAecPl1GUkOtHXelGeUD00KiErheuHr1kC-xQu_LMSpW8caGivXfoo7oEI7LdV-_IgOYuiNP_02inN5UMbsLhPQ_KTketP6yLGbETWd9T-vK5LhbHqrLdxVmSyFIpEVaJR61Q" alt="Logo" class="w-24 h-24 mx-auto rounded-2xl shadow-xl border border-slate-700">
                <span class="inline-block px-3 py-1 bg-emerald-500/10 text-emerald-400 text-xs font-semibold rounded-full border border-emerald-500/20">Slide 1 de 11</span>
                <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-100 leading-tight">Uma operação digital preparada para crescer com método.</h2>
                <p class="text-sm sm:text-base text-slate-400 max-w-md mx-auto">Plataforma em produção. Processos em evolução. Crescimento por etapas.</p>
            </div>
            <div class="p-4 bg-emerald-950/30 border border-emerald-500/30 rounded-xl text-xs text-emerald-300 flex items-start gap-3">
                <i class="fa-solid fa-lightbulb mt-0.5 text-emerald-400 text-sm"></i>
                <div><strong>Ideia central:</strong> O crescimento sustentável não depende de apenas acumular cadastros, mas de fazer cada etapa da jornada operar e ser mensurável.</div>
            </div>
        </div>

        <!-- Slide 2 -->
        <div class="slide-card space-y-5 hidden" id="slide-2">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 2 • Visão Estratégica</span>
                <h2 class="text-xl sm:text-2xl font-bold">A Ambição</h2>
                <p class="text-xs sm:text-sm text-slate-400">Crescer é transformar atividade em resultado recorrente</p>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 text-xs">
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-emerald-400">1. Atração</span>
                    <p class="text-slate-300 mt-1">Atrair vendedores e compradores por canais identificáveis.</p>
                </div>
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-amber-400">2. Preparação</span>
                    <p class="text-slate-300 mt-1">Preparar lojas para operar e vender de verdade.</p>
                </div>
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-orange-400">3. Pedidos</span>
                    <p class="text-slate-300 mt-1">Gerar pedidos reais e acompanhar a experiência.</p>
                </div>
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-blue-400">4. Aprendizado</span>
                    <p class="text-slate-300 mt-1">Aprender com os resultados antes de ampliar.</p>
                </div>
            </div>
            <div class="p-4 bg-gradient-to-r from-emerald-950/40 via-amber-950/40 to-orange-950/40 border border-amber-500/30 rounded-xl text-center">
                <p class="text-xs sm:text-sm font-semibold text-amber-200">"Cadastro é o começo do processo — não a medida do crescimento."</p>
            </div>
        </div>

        <!-- Slide 3 -->
        <div class="slide-card space-y-5 hidden" id="slide-3">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 3 • Diagnóstico</span>
                <h2 class="text-xl sm:text-2xl font-bold">O Desafio Operacional</h2>
                <p class="text-xs sm:text-sm text-slate-400">Uma plataforma precisa de demanda e execução</p>
            </div>
            <div class="space-y-3 text-xs">
                <div class="p-4 bg-slate-800/60 border-l-4 border-emerald-500 rounded-r-lg space-y-2">
                    <span class="font-bold text-emerald-400 text-sm">Do lado dos Vendedores</span>
                    <ul class="list-disc list-inside space-y-1 text-slate-300">
                        <li>Cadastro não garante que a loja esteja pronta.</li>
                        <li>Loja pronta não garante que a primeira venda aconteça.</li>
                        <li>Uma venda isolada ainda não prova recorrência.</li>
                    </ul>
                </div>
                <div class="p-4 bg-slate-800/60 border-l-4 border-orange-500 rounded-r-lg space-y-2">
                    <span class="font-bold text-orange-400 text-sm">Do lado dos Compradores</span>
                    <ul class="list-disc list-inside space-y-1 text-slate-300">
                        <li>Atrair vendedores, por si só, não garante demanda.</li>
                        <li>É preciso identificar quais canais trazem tráfego real.</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Slide 4 -->
        <div class="slide-card space-y-4 hidden" id="slide-4">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 4 • Metodologia</span>
                <h2 class="text-xl sm:text-2xl font-bold">A Arquitetura de Crescimento</h2>
                <p class="text-xs sm:text-sm text-slate-400">Cinco etapas em ciclo de aprendizagem contínua</p>
            </div>
            <div class="space-y-2 text-xs">
                <div class="flex items-center gap-3 p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="w-6 h-6 rounded-full bg-emerald-500 text-slate-900 font-bold flex items-center justify-center shrink-0">1</span>
                    <div><strong class="text-slate-100">Captação:</strong> Atrair vendedores e clientes por canais identificáveis.</div>
                </div>
                <div class="flex items-center gap-3 p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="w-6 h-6 rounded-full bg-emerald-600 text-slate-900 font-bold flex items-center justify-center shrink-0">2</span>
                    <div><strong class="text-slate-100">Cadastro & Ativação:</strong> Preparar a loja e confirmar aptidão.</div>
                </div>
                <div class="flex items-center gap-3 p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="w-6 h-6 rounded-full bg-amber-500 text-slate-900 font-bold flex items-center justify-center shrink-0">3</span>
                    <div><strong class="text-slate-100">Primeira Venda:</strong> Gerar visitas, pedidos reais e boa experiência.</div>
                </div>
                <div class="flex items-center gap-3 p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="w-6 h-6 rounded-full bg-orange-500 text-slate-900 font-bold flex items-center justify-center shrink-0">4</span>
                    <div><strong class="text-slate-100">Retenção & Recorrência:</strong> Estimular a permanência e retorno.</div>
                </div>
                <div class="flex items-center gap-3 p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="w-6 h-6 rounded-full bg-blue-500 text-slate-900 font-bold flex items-center justify-center shrink-0">5</span>
                    <div><strong class="text-slate-100">Medição & Expansão:</strong> Identificar o que funciona e replicar.</div>
                </div>
            </div>
        </div>

        <!-- Slide 5 -->
        <div class="slide-card space-y-4 hidden" id="slide-5">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 5 • Ativação</span>
                <h2 class="text-xl sm:text-2xl font-bold">Experiência Padronizada</h2>
                <p class="text-xs sm:text-sm text-slate-400">Trilha operacional do vendedor</p>
            </div>
            <div class="space-y-2 text-xs">
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg flex justify-between items-center">
                    <span><strong>1. Entrada:</strong> Registrar origem e canal</span>
                    <span class="text-[10px] bg-emerald-500/20 text-emerald-400 px-2 py-0.5 rounded">Contato Registrado</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg flex justify-between items-center">
                    <span><strong>2. Cadastro:</strong> Dados mínimos necessários</span>
                    <span class="text-[10px] bg-emerald-500/20 text-emerald-400 px-2 py-0.5 rounded">Cadastro Criado</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg flex justify-between items-center">
                    <span><strong>3. Preparação:</strong> Aplicar modelo por segmento</span>
                    <span class="text-[10px] bg-amber-500/20 text-amber-400 px-2 py-0.5 rounded">Loja Conferida</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg flex justify-between items-center">
                    <span><strong>4. Teste:</strong> Conferir vitrine e fluxo</span>
                    <span class="text-[10px] bg-amber-500/20 text-amber-400 px-2 py-0.5 rounded">Loja Apta</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg flex justify-between items-center">
                    <span><strong>5. Acompanhamento:</strong> Agir sobre gargalos</span>
                    <span class="text-[10px] bg-orange-500/20 text-orange-400 px-2 py-0.5 rounded">Plano de Ativação</span>
                </div>
            </div>
        </div>

        <!-- Slide 6 -->
        <div class="slide-card space-y-4 hidden" id="slide-6">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 6 • Frentes Simultâneas</span>
                <h2 class="text-xl sm:text-2xl font-bold">Oferta e Demanda</h2>
                <p class="text-xs sm:text-sm text-slate-400">Avançando juntas no sistema</p>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 text-xs">
                <div class="p-3 bg-slate-800/60 border border-emerald-500/30 rounded-lg space-y-1">
                    <span class="font-bold text-emerald-400">Vendedores (Oferta)</span>
                    <ul class="list-disc list-inside text-slate-300 space-y-1">
                        <li>Identificar origem dos contatos</li>
                        <li>Simplificar o cadastro</li>
                        <li>Padrões visuais por segmento</li>
                        <li>Acompanhar ativação e 1ª venda</li>
                    </ul>
                </div>
                <div class="p-3 bg-slate-800/60 border border-orange-500/30 rounded-lg space-y-1">
                    <span class="font-bold text-orange-400">Compradores (Demanda)</span>
                    <ul class="list-disc list-inside text-slate-300 space-y-1">
                        <li>Registrar campanhas/origens</li>
                        <li>Medir tráfego e início de pedidos</li>
                        <li>Medir concluídos e cancelados</li>
                        <li>Analisar retorno e atribuição</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Slide 7 -->
        <div class="slide-card space-y-4 hidden" id="slide-7">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 7 • Organização</span>
                <h2 class="text-xl sm:text-2xl font-bold">Operação Independente de Pessoas</h2>
                <p class="text-xs sm:text-sm text-slate-400">Funções claras e conhecimento documentado</p>
            </div>
            <div class="grid grid-cols-2 sm:grid-cols-3 gap-2 text-[11px]">
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <strong class="text-emerald-400 block mb-0.5">Gestão Geral</strong>
                    Definir prioridades, orçamento e metas.
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <strong class="text-emerald-400 block mb-0.5">Operação Campo</strong>
                    Atrair vendedores e apoiar cadastros.
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <strong class="text-amber-400 block mb-0.5">Ativação</strong>
                    Preparar lojas e acompanhar 1ª venda.
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <strong class="text-amber-400 block mb-0.5">Marketing</strong>
                    Atrair compradores e gerar demanda.
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <strong class="text-orange-400 block mb-0.5">Tecnologia</strong>
                    Preservar produção e evoluir.
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <strong class="text-orange-400 block mb-0.5">Análise Dados</strong>
                    Medir indicadores e propor correções.
                </div>
            </div>
        </div>

        <!-- Slide 8 -->
        <div class="slide-card space-y-4 hidden" id="slide-8">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 8 • Evidências</span>
                <h2 class="text-xl sm:text-2xl font-bold">Crescimento Orientado a Dados</h2>
                <p class="text-xs sm:text-sm text-slate-400">Primeiro medir. Depois definir metas.</p>
            </div>
            <div class="grid grid-cols-2 sm:grid-cols-3 gap-2 text-xs">
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="text-slate-400 block text-[10px]">Custo por Ativação</span>
                    <span class="font-semibold text-emerald-400">Em medição</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="text-slate-400 block text-[10px]">Taxa de 1ª Venda</span>
                    <span class="font-semibold text-emerald-400">Em medição</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="text-slate-400 block text-[10px]">Atividade Semanal</span>
                    <span class="font-semibold text-amber-400">A estabelecer</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="text-slate-400 block text-[10px]">Conversão Comprador</span>
                    <span class="font-semibold text-amber-400">A estabelecer</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="text-slate-400 block text-[10px]">Taxa Recorrência</span>
                    <span class="font-semibold text-orange-400">Em medição</span>
                </div>
                <div class="p-2.5 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="text-slate-400 block text-[10px]">Margem Contribuição</span>
                    <span class="font-semibold text-orange-400">A estabelecer</span>
                </div>
            </div>
        </div>

        <!-- Slide 9 -->
        <div class="slide-card space-y-4 hidden" id="slide-9">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 9 • Tecnologia</span>
                <h2 class="text-xl sm:text-2xl font-bold">Evolução com Controle de Risco</h2>
                <p class="text-xs sm:text-sm text-slate-400">Evoluir sem quebrar o que funciona</p>
            </div>
            <div class="space-y-2 text-xs">
                <div class="p-2.5 bg-slate-800/60 border-l-4 border-emerald-500 rounded-r-lg">
                    <strong class="text-emerald-400">Fase A: Proteger Produção</strong>
                    <p class="text-slate-300">Documentar e testar carrinho, pedidos e pagamentos.</p>
                </div>
                <div class="p-2.5 bg-slate-800/60 border-l-4 border-emerald-600 rounded-r-lg">
                    <strong class="text-emerald-300">Fase B: Preparar Lojas</strong>
                    <p class="text-slate-300">Criar painel administrativo interno padronizado.</p>
                </div>
                <div class="p-2.5 bg-slate-800/60 border-l-4 border-amber-500 rounded-r-lg">
                    <strong class="text-amber-400">Fase C: Digitalizar Captação</strong>
                    <p class="text-slate-300">Links rastreáveis e cadastro simplificado.</p>
                </div>
                <div class="p-2.5 bg-slate-800/60 border-l-4 border-orange-500 rounded-r-lg">
                    <strong class="text-orange-400">Fase D: Atrair Compradores</strong>
                    <p class="text-slate-300">Medir tráfego, conversão e recompra por campanha.</p>
                </div>
                <div class="p-2.5 bg-slate-800/60 border-l-4 border-blue-500 rounded-r-lg">
                    <strong class="text-blue-400">Fase E: Automatizar</strong>
                    <p class="text-slate-300">Automatizar tarefas após validar processos.</p>
                </div>
            </div>
        </div>

        <!-- Slide 10 -->
        <div class="slide-card space-y-4 hidden" id="slide-10">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 10 • Plano de Ação</span>
                <h2 class="text-xl sm:text-2xl font-bold">Primeiros 30 Dias</h2>
                <p class="text-xs sm:text-sm text-slate-400">Ciclo inicial de validação</p>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 text-xs">
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-emerald-400">Dias 1–7 | Organizar</span>
                    <p class="text-slate-300 mt-1">Documentar processo, identificar falhas e criar linhas de base.</p>
                </div>
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-emerald-300">Dias 8–14 | Padronizar</span>
                    <p class="text-slate-300 mt-1">Modelos de loja e rotina de acompanhamento com grupo teste.</p>
                </div>
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-amber-400">Dias 15–21 | Validar Captação</span>
                    <p class="text-slate-300 mt-1">Testar cadastro digital com grupo controlado e medir desistências.</p>
                </div>
                <div class="p-3 bg-slate-800/60 border border-slate-700/60 rounded-lg">
                    <span class="font-bold text-orange-400">Dias 22–30 | Validar Vendas</span>
                    <p class="text-slate-300 mt-1">Testes de aquisição de compradores e medição de recompra.</p>
                </div>
            </div>
        </div>

        <!-- Slide 11 -->
        <div class="slide-card space-y-5 hidden" id="slide-11">
            <div class="space-y-1">
                <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Slide 11 • Conclusão</span>
                <h2 class="text-xl sm:text-2xl font-bold">Decisão e Próximo Passo</h2>
                <p class="text-xs sm:text-sm text-slate-400">Começar pelo que cria base de escala</p>
            </div>
            <div class="p-4 bg-emerald-950/40 border border-emerald-500/40 rounded-xl space-y-2 text-xs">
                <strong class="text-emerald-400 text-sm">Recomendação Inicial:</strong>
                <p class="text-slate-200">Iniciar pelo painel interno de preparação de lojas, após auditar a arquitetura e fluxos atuais.</p>
            </div>
            <div class="space-y-1.5 text-xs text-slate-300">
                <div class="flex gap-2"><span>1.</span><span>Auditar operação em produção</span></div>
                <div class="flex gap-2"><span>2.</span><span>Especificar o painel e validar processo</span></div>
                <div class="flex gap-2"><span>3.</span><span>Implementar e testar de forma isolada</span></div>
                <div class="flex gap-2"><span>4.</span><span>Conectar preparação à captação digital</span></div>
                <div class="flex gap-2"><span>5.</span><span>Avançar para aquisição de compradores</span></div>
            </div>
            <div class="p-4 bg-slate-800/80 rounded-xl border border-slate-700 text-center">
                <p class="text-xs font-bold text-amber-300">"Construir não apenas funcionalidades, mas uma operação capaz de crescer com método."</p>
            </div>
        </div>

    </main>

    <!-- Footer Fixo de Navegação Mobile -->
    <footer class="sticky bottom-0 bg-slate-900/95 backdrop-blur-md border-t border-slate-800 px-4 py-3 flex items-center justify-between z-50">
        <button id="prevBtn" onclick="changeSlide(-1)" class="px-4 py-2 bg-slate-800 text-slate-300 rounded-lg text-xs font-semibold hover:bg-slate-700 disabled:opacity-40 disabled:cursor-not-allowed border border-slate-700 flex items-center gap-2">
            <i class="fa-solid fa-chevron-left"></i> Anterior
        </button>
        
        <span id="slideCounter" class="text-xs font-bold text-slate-400">1 / 11</span>

        <button id="nextBtn" onclick="changeSlide(1)" class="px-4 py-2 bg-emerald-600 text-white rounded-lg text-xs font-semibold hover:bg-emerald-500 border border-emerald-500/50 flex items-center gap-2 shadow-lg shadow-emerald-950/50">
            Próximo <i class="fa-solid fa-chevron-right"></i>
        </button>
    </footer>

    <script>
        let currentSlide = 1;
        const totalSlides = 11;
        let isDarkMode = true;
        let fontScale = 100;

        function updateSlide() {
            for (let i = 1; i <= totalSlides; i++) {
                const slide = document.getElementById(`slide-${i}`);
                if (i === currentSlide) {
                    slide.classList.remove('hidden');
                } else {
                    slide.classList.add('hidden');
                }
            }

            document.getElementById('slideCounter').innerText = `${currentSlide} / ${totalSlides}`;
            document.getElementById('progressBar').style.width = `${(currentSlide / totalSlides) * 100}%`;

            document.getElementById('prevBtn').disabled = currentSlide === 1;
            
            const nextBtn = document.getElementById('nextBtn');
            if (currentSlide === totalSlides) {
                nextBtn.innerHTML = 'Finalizar <i class="fa-solid fa-check"></i>';
                nextBtn.className = "px-4 py-2 bg-amber-600 text-white rounded-lg text-xs font-semibold hover:bg-amber-500 border border-amber-500/50 flex items-center gap-2";
            } else {
                nextBtn.innerHTML = 'Próximo <i class="fa-solid fa-chevron-right"></i>';
                nextBtn.className = "px-4 py-2 bg-emerald-600 text-white rounded-lg text-xs font-semibold hover:bg-emerald-500 border border-emerald-500/50 flex items-center gap-2";
            }

            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function changeSlide(direction) {
            if (currentSlide + direction >= 1 && currentSlide + direction <= totalSlides) {
                currentSlide += direction;
                updateSlide();
            }
        }

        function adjustFontSize(delta) {
            fontScale = Math.min(Math.max(fontScale + (delta * 10), 80), 140);
            document.querySelector('main').style.fontSize = `${fontScale}%`;
        }

        function toggleTheme() {
            isDarkMode = !isDarkMode;
            const body = document.body;
            const themeIcon = document.getElementById('themeIcon');
            const themeLabel = document.getElementById('themeLabel');

            if (isDarkMode) {
                body.className = "bg-slate-900 text-slate-100 min-h-screen flex flex-col justify-between selection:bg-emerald-500 selection:text-white";
                themeIcon.className = "fa-solid fa-sun";
                themeLabel.innerText = "Modo Claro";
            } else {
                body.className = "bg-slate-50 text-slate-800 min-h-screen flex flex-col justify-between selection:bg-emerald-500 selection:text-white";
                themeIcon.className = "fa-solid fa-moon";
                themeLabel.innerText = "Modo Escuro";
            }
        }

        // Suporte para navegação por gesto Swipe no celular
        let touchstartX = 0;
        let touchendX = 0;
            
        function handleGesture() {
            if (touchendX < touchstartX - 50) changeSlide(1);
            if (touchendX > touchstartX + 50) changeSlide(-1);
        }

        document.addEventListener('touchstart', e => {
            touchstartX = e.changedTouches[0].screenX;
        });

        document.addEventListener('touchend', e => {
            touchendX = e.changedTouches[0].screenX;
            handleGesture();
        });

        updateSlide();
    </script>
</body>
</html>