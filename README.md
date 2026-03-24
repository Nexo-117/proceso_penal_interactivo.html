<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proceso Penal: Etapas y Actos Procesales</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root {
            --bg-main: #f8fafc;
            --investigacion: #3b82f6;
            --intermedia: #10b981;
            --juicio: #f59e0b;
        }
        body {
            background-color: var(--bg-main);
            font-family: 'Inter', system-ui, -apple-system, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }
        .node-card {
            transition: all 0.4s cubic-bezier(0.23, 1, 0.32, 1);
        }
        .node-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
        }
        .etapa-header { border-left-width: 6px; }
        .investigacion { border-color: var(--investigacion); }
        .intermedia { border-color: var(--intermedia); }
        .juicio { border-color: var(--juicio); }
        
        .custom-scrollbar::-webkit-scrollbar { width: 6px; }
        .custom-scrollbar::-webkit-scrollbar-track { background: #f1f1f1; }
        .custom-scrollbar::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 10px; }
    </style>
</head>
<body class="p-4 md:p-12 min-h-screen">

    <header class="max-w-6xl mx-auto mb-16 text-center">
        <span class="inline-block px-3 py-1 text-xs font-semibold tracking-widest text-blue-600 uppercase bg-blue-100 rounded-full mb-4">
            Derecho Procesal Penal
        </span>
        <h1 class="text-4xl md:text-5xl font-black text-slate-900 mb-4 tracking-tight">
            Mapa Mental Interactivo
        </h1>
        <div class="h-1 w-24 bg-slate-800 mx-auto rounded-full mb-4"></div>
        <p class="text-slate-500 max-w-2xl mx-auto text-lg">
            Explora las etapas y actos del proceso penal mediante este Altar Racional interactivo.
        </p>
    </header>

    <main class="max-w-7xl mx-auto grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
        
        <!-- Etapa 1: Investigación Inicial -->
        <div onclick="showDetails('investigacion-inicial')" class="node-card bg-white p-8 rounded-3xl shadow-sm etapa-header investigacion border-l-6 cursor-pointer group">
            <div class="flex justify-between items-start mb-6">
                <div class="p-3 bg-blue-50 rounded-2xl text-blue-600 group-hover:bg-blue-600 group-hover:text-white transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                    </svg>
                </div>
            </div>
            <h2 class="text-2xl font-bold text-slate-800 mb-2">Investigación Inicial</h2>
            <p class="text-slate-500 text-sm mb-6 leading-relaxed">Etapa de esclarecimiento y determinación delictiva.</p>
            <span class="text-blue-600 font-semibold text-xs uppercase tracking-wider flex items-center">
                Ver detalles 
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
            </span>
        </div>

        <!-- Etapa 2: Investigación Complementaria -->
        <div onclick="showDetails('investigacion-complementaria')" class="node-card bg-white p-8 rounded-3xl shadow-sm etapa-header investigacion border-l-6 cursor-pointer group">
            <div class="flex justify-between items-start mb-6">
                <div class="p-3 bg-blue-50 rounded-2xl text-blue-500 group-hover:bg-blue-500 group-hover:text-white transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
                    </svg>
                </div>
            </div>
            <h2 class="text-2xl font-bold text-slate-800 mb-2">Investigación Complementaria</h2>
            <p class="text-slate-500 text-sm mb-6 leading-relaxed">Robustecimiento del caso tras vinculación.</p>
            <span class="text-blue-500 font-semibold text-xs uppercase tracking-wider flex items-center">
                Ver detalles 
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
            </span>
        </div>

        <!-- Etapa 3: Etapa Intermedia -->
        <div onclick="showDetails('etapa-intermedia')" class="node-card bg-white p-8 rounded-3xl shadow-sm etapa-header intermedia border-l-6 cursor-pointer group">
            <div class="flex justify-between items-start mb-6">
                <div class="p-3 bg-emerald-50 rounded-2xl text-emerald-600 group-hover:bg-emerald-600 group-hover:text-white transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
                    </svg>
                </div>
            </div>
            <h2 class="text-2xl font-bold text-slate-800 mb-2">Etapa Intermedia</h2>
            <p class="text-slate-500 text-sm mb-6 leading-relaxed">Filtro de pruebas y preparación a juicio.</p>
            <span class="text-emerald-600 font-semibold text-xs uppercase tracking-wider flex items-center">
                Ver detalles 
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
            </span>
        </div>

        <!-- Etapa 4: Juicio Oral -->
        <div onclick="showDetails('juicio-oral')" class="node-card bg-white p-8 rounded-3xl shadow-sm etapa-header juicio border-l-6 cursor-pointer group">
            <div class="flex justify-between items-start mb-6">
                <div class="p-3 bg-amber-50 rounded-2xl text-amber-600 group-hover:bg-amber-600 group-hover:text-white transition-colors">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 6l3 1m0 0l-3 9a5.002 5.002 0 006.001 0M6 7l3 9M6 7l6-2m6 2l3-1m-3 1l-3 9a5.002 5.002 0 006.001 0M18 7l3 9m-3-9l-6-2m0-2v2m0 16V5m0 16H9m3 0h3" />
                    </svg>
                </div>
            </div>
            <h2 class="text-2xl font-bold text-slate-800 mb-2">Juicio Oral</h2>
            <p class="text-slate-500 text-sm mb-6 leading-relaxed">Determinación de culpabilidad o inocencia.</p>
            <span class="text-amber-600 font-semibold text-xs uppercase tracking-wider flex items-center">
                Ver detalles 
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
            </span>
        </div>

    </main>

    <!-- Modal Overlay -->
    <div id="modal" class="fixed inset-0 bg-slate-900/60 backdrop-blur-md hidden flex items-center justify-center p-4 z-50 transition-opacity duration-300">
        <div id="modal-content" class="bg-white rounded-[2.5rem] max-w-2xl w-full max-h-[85vh] overflow-y-auto p-10 shadow-2xl custom-scrollbar relative">
            <!-- Dynamic Content -->
        </div>
    </div>

    <script>
        const data = {
            'investigacion-inicial': {
                title: 'Investigación Inicial',
                color: 'text-blue-700',
                objetivo: 'Iniciar el esclarecimiento de los hechos tras una denuncia para determinar si se cometió un delito.',
                sujetos: 'Ministerio Público (MP), víctima, asesor jurídico, imputado y defensor. Interviene el Juez de Control.',
                actos: [
                    '<strong>Denuncia:</strong> Acto que da inicio a la etapa.',
                    '<strong>Control de detención:</strong> El juez verifica legalidad en flagrancia.',
                    '<strong>Formulación de imputación:</strong> Notificación oficial de los hechos investigados.',
                    '<strong>Declaración del imputado:</strong> Derecho a declarar o guardar silencio.',
                    '<strong>Vinculación a proceso:</strong> Determinación de indicios razonables de participación.',
                    '<strong>Medidas cautelares:</strong> Solicitadas para asegurar el proceso o proteger víctimas.'
                ],
                plazos: '72 horas para resolver situación jurídica, prorrogable a 144 horas.'
            },
            'investigacion-complementaria': {
                title: 'Investigación Complementaria',
                color: 'text-blue-500',
                objetivo: 'Permitir al Ministerio Público y a la defensa recabar más pruebas tras la vinculación.',
                sujetos: 'MP, defensa e imputado supervisados por el Juez.',
                actos: [
                    'Realización de peritajes técnicos.',
                    'Recopilación de testimonios adicionales.',
                    'Integración de registros a la carpeta de investigación.',
                    'Cierre de la investigación formal.'
                ],
                plazos: 'El plazo lo fija el juez; no mayor a 2 meses (delito pena < 2 años) o 6 meses (delito pena > 2 años).'
            },
            'etapa-intermedia': {
                title: 'Etapa Intermedia',
                color: 'text-emerald-600',
                objetivo: 'Depuración de hechos y admisión de medios de prueba para el juicio.',
                sujetos: 'Juez de Control, MP, defensa y víctimas.',
                actos: [
                    '<strong>Escrito de Acusación:</strong> Formalización de la pretensión punitiva.',
                    '<strong>Descubrimiento probatorio:</strong> Intercambio de evidencias entre partes.',
                    '<strong>Exclusiones:</strong> Eliminación de pruebas ilícitas o impertinentes.',
                    '<strong>Auto de apertura:</strong> Resolución que envía el caso a Juicio Oral.',
                    '<strong>Salidas Alternas:</strong> Última oportunidad para Acuerdos Reparatorios.'
                ]
            },
            'juicio-oral': {
                title: 'Juicio Oral',
                color: 'text-amber-600',
                objetivo: 'Desahogo de pruebas ante un Tribunal de Enjuiciamiento para emitir sentencia.',
                sujetos: 'Tribunal (1 o 3 jueces), partes procesales y testigos/peritos.',
                actos: [
                    '<strong>Alegatos de apertura:</strong> Presentación de la teoría del caso.',
                    '<strong>Desahogo:</strong> Interrogatorio y contrainterrogatorio de testigos.',
                    '<strong>Sentencia:</strong> Fallo condenatorio o absolutorio.',
                    '<strong>Individualización:</strong> Audiencia específica para fijar la magnitud de la pena.'
                ],
                plazos: 'Sentencia debe dictarse máximo en 2 años. 10 días para apelación.'
            }
        };

        function showDetails(key) {
            const entry = data[key];
            const modal = document.getElementById('modal');
            const content = document.getElementById('modal-content');
            
            content.innerHTML = `
                <button onclick="closeModal()" class="absolute top-6 right-6 text-slate-400 hover:text-slate-900 transition-colors p-2 rounded-full hover:bg-slate-100">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                    </svg>
                </button>
                
                <h2 class="text-3xl font-black ${entry.color} mb-8 pr-12">${entry.title}</h2>
                
                <div class="space-y-8">
                    <section class="animate-fade-in">
                        <h3 class="text-[10px] font-black text-slate-400 uppercase tracking-[0.2em] mb-3">Objetivo Sistémico</h3>
                        <p class="text-slate-700 leading-relaxed text-lg">${entry.objetivo}</p>
                    </section>
                    
                    <section>
                        <h3 class="text-[10px] font-black text-slate-400 uppercase tracking-[0.2em] mb-3">Sujetos Involucrados</h3>
                        <p class="text-slate-600">${entry.sujetos}</p>
                    </section>

                    <section>
                        <h3 class="text-[10px] font-black text-slate-400 uppercase tracking-[0.2em] mb-4">Actos Procesales Clave</h3>
                        <div class="grid gap-3">
                            ${entry.actos.map(a => `
                                <div class="flex items-start p-3 bg-slate-50 rounded-xl border border-slate-100">
                                    <div class="mt-1.5 h-1.5 w-1.5 rounded-full bg-slate-400 flex-shrink-0 mr-3"></div>
                                    <span class="text-slate-700 text-sm leading-snug">${a}</span>
                                </div>
                            `).join('')}
                        </div>
                    </section>

                    ${entry.plazos ? `
                    <section class="bg-slate-900 p-6 rounded-2xl text-white">
                        <h3 class="text-[10px] font-black text-slate-500 uppercase tracking-[0.2em] mb-2">Restricción Temporal</h3>
                        <p class="text-sm font-medium">${entry.plazos}</p>
                    </section>
                    ` : ''}
                </div>
            `;

            modal.classList.remove('hidden');
            setTimeout(() => modal.classList.add('opacity-100'), 10);
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            const modal = document.getElementById('modal');
            modal.classList.remove('opacity-100');
            setTimeout(() => modal.classList.add('hidden'), 300);
            document.body.style.overflow = 'auto';
        }

        window.onclick = function(event) {
            if (event.target == document.getElementById('modal')) closeModal();
        }
    </script>
</body>
</html>

