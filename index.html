<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistema de Gallos Pro 2026 - Control Total</title>
    <style>
        :root { --primary: #0f172a; --secondary: #e11d48; --accent: #10b981; --bg: #f8fafc; --card: #ffffff; }
        body { font-family: 'Inter', system-ui, sans-serif; background: var(--bg); color: #1e293b; margin: 0; padding: 20px; }
        .container { max-width: 1100px; margin: auto; background: var(--card); padding: 25px; border-radius: 16px; box-shadow: 0 4px 20px rgba(0,0,0,0.08); }
        .header-top { display: flex; justify-content: space-between; align-items: center; border-bottom: 2px solid #e2e8f0; margin-bottom: 25px; padding-bottom: 10px; }
        
        /* Panel de Registro */
        .panel { display: grid; grid-template-columns: repeat(auto-fit, minmax(110px, 1fr)); gap: 8px; background: #f1f5f9; padding: 15px; border-radius: 12px; }
        input, select { padding: 10px; border: 1px solid #cbd5e1; border-radius: 6px; font-size: 0.85rem; width: 100%; box-sizing: border-box; }
        
        .btn { padding: 10px 15px; border: none; border-radius: 6px; font-weight: 600; cursor: pointer; transition: all 0.2s; }
        .btn-add { background: var(--accent); color: white; }
        .btn-match { background: var(--primary); color: white; width: 100%; margin: 20px 0; font-size: 1rem; }
        .btn-reset { background: var(--secondary); color: white; font-size: 0.8rem; }
        
        table { width: 100%; border-collapse: collapse; margin-top: 20px; font-size: 0.85rem; }
        th { background: #f8fafc; color: #64748b; text-align: left; padding: 12px; border-bottom: 2px solid #e2e8f0; }
        td { padding: 12px; border-bottom: 1px solid #f1f5f9; }
        
        /* TARJETAS DE PELEA OPTIMIZADAS */
        .match-card { border: 2px solid #0f172a; border-radius: 12px; margin-bottom: 25px; overflow: hidden; background: white; page-break-inside: avoid; }
        .match-header { background: #0f172a; color: white; padding: 8px 15px; font-size: 0.85rem; display: flex; justify-content: space-between; font-weight: bold; }
        .match-info { display: grid; grid-template-columns: 1fr 40px 1fr; align-items: center; padding: 15px; gap: 10px; background: #fff; }
        .vs { font-weight: 900; color: var(--secondary); font-size: 1.2rem; text-align: center; }
        
        .gallo-box { padding: 8px; border-radius: 8px; background: #fdfdfd; }
        .gallo-box b { font-size: 1.1rem; color: #0f172a; display: block; margin-bottom: 8px; text-transform: uppercase; border-bottom: 1px solid #eee; padding-bottom: 3px; }
        
        /* Rejilla de información técnica */
        .info-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 6px; }
        .info-item { background: #f1f5f9; padding: 4px 6px; border-radius: 4px; font-size: 0.72rem; font-weight: 600; color: #334155; border: 1px solid #e2e8f0; }
        .info-item span { color: #64748b; font-weight: 400; display: block; font-size: 0.65rem; text-transform: uppercase; }

        .result-zone { background: #f8fafc; padding: 12px; display: flex; flex-wrap: wrap; gap: 15px; justify-content: center; align-items: center; border-top: 1px solid #e2e8f0; }
        .time-group { display: flex; align-items: center; gap: 5px; font-weight: bold; font-size: 0.9rem; }
        .time-group input { width: 55px; padding: 5px; text-align: center; }

        .leader-row { background: #f0fdf4 !important; font-weight: bold; }

        @media print { 
            .no-print { display: none !important; } 
            .container { box-shadow: none; border: none; width: 100%; padding: 0; }
            body { background: white; padding: 0; }
            .match-card { border: 1px solid #000; margin-bottom: 15px; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header-top">
        <h1>🏆 GALLOS PRO <span style="font-weight: 300;">v2026</span></h1>
        <button class="btn btn-reset no-print" onclick="resetearSistema()">🧹 LIMPIAR TODO EL SISTEMA</button>
    </div>

    <div class="panel no-print">
        <input type="text" id="cuerda" placeholder="Cuerda">
        <input type="number" id="frente" placeholder="Frente #" value="1">
        <input type="text" id="placa" placeholder="Placa">
        <input type="text" id="anillo" placeholder="Anillo">
        <input type="number" id="peso" placeholder="Peso" step="0.01">
        <select id="marca">
            <option value="">Mes Nac.</option>
            <option value="Ene">Ene</option><option value="Feb">Feb</option><option value="Mar">Mar</option>
            <option value="Abr">Abr</option><option value="May">May</option><option value="Jun">Jun</option>
            <option value="Jul">Jul</option><option value="Ago">Ago</option><option value="Sep">Sep</option>
            <option value="Oct">Oct</option><option value="Nov">Nov</option><option value="Dic">Dic</option>
        </select>
        <button class="btn btn-add" onclick="registrarGallo()">➕ Registrar</button>
    </div>

    <table id="tablaGallos" class="no-print">
        <thead>
            <tr><th>Cuerda</th><th>Fte</th><th>Placa</th><th>Anillo</th><th>Peso</th><th>Mes</th><th></th></tr>
        </thead>
        <tbody id="tbodyGallos"></tbody>
    </table>

    <button class="btn btn-match no-print" onclick="generarEnfrentamientos()">⚔️ CASAR PELEAS POR PESO</button>

    <div id="resultadosCotejo"></div>

    <div id="seccionEstadisticas" style="display:none; margin-top: 40px;">
        <h2 style="text-align:center">📊 RANKING POR FRENTES</h2>
        <table id="tablaEstadisticas">
            <thead>
                <tr><th>Cuerda - Frente</th><th>Inscritos</th><th>G</th><th>P</th><th>T</th><th>Puntos</th><th>Tiempo Total</th></tr>
            </thead>
            <tbody></tbody>
        </table>
        <div class="no-print" style="margin-top: 20px; display: flex; gap: 10px;">
            <button class="btn btn-match" style="background:var(--accent)" onclick="actualizarEstadisticas()">🔄 Actualizar Tabla</button>
            <button class="btn btn-match" style="background: #334155" onclick="window.print()">🖨️ Imprimir Todo</button>
        </div>
    </div>
</div>

<script>
    let gallos = JSON.parse(localStorage.getItem('gallos')) || [];
    let peleasCasadas = JSON.parse(localStorage.getItem('peleas')) || [];

    window.onload = () => {
        actualizarTabla();
        if(peleasCasadas.length > 0) {
            renderizarTodasPeleas();
            actualizarEstadisticas();
            document.getElementById('seccionEstadisticas').style.display = 'block';
        }
    };

    function registrarGallo() {
        const cuerda = document.getElementById('cuerda').value.toUpperCase().trim();
        const frente = document.getElementById('frente').value;
        const peso = parseFloat(document.getElementById('peso').value);
        const placa = document.getElementById('placa').value || "S/P";
        const anillo = document.getElementById('anillo').value || "S/A";
        const marca = document.getElementById('marca').value || "N/A";

        if(!cuerda || isNaN(peso)) return alert("Nombre de Cuerda y Peso son obligatorios.");

        gallos.push({ id: Date.now(), cuerda, frente, placa, anillo, peso, marca });
        localStorage.setItem('gallos', JSON.stringify(gallos));
        actualizarTabla();
        document.getElementById('placa').value = "";
        document.getElementById('anillo').value = "";
        document.getElementById('peso').value = "";
    }

    function actualizarTabla() {
        const tbody = document.getElementById("tbodyGallos");
        tbody.innerHTML = gallos.map((g, i) => `
            <tr><td><b>${g.cuerda}</b></td><td>F-${g.frente}</td><td>${g.placa}</td><td>${g.anillo}</td><td>${g.peso.toFixed(2)}</td><td>${g.marca}</td><td><button onclick="eliminarGallo(${i})" style="color:red; background:none; border:none; cursor:pointer;">✕</button></td></tr>
        `).join('');
    }

    function eliminarGallo(i) {
        gallos.splice(i, 1);
        localStorage.setItem('gallos', JSON.stringify(gallos));
        actualizarTabla();
    }

    function generarEnfrentamientos() {
        if(gallos.length < 2) return alert("No hay suficientes gallos para cotejar.");
        let disponibles = [...gallos].sort((a, b) => a.peso - b.peso);
        peleasCasadas = [];
        let contador = 1;
        const margenes = [0.02, 0.05, 0.10, 0.15, 0.20];

        margenes.forEach(margen => {
            for (let i = 0; i < disponibles.length; i++) {
                for (let j = i + 1; j < disponibles.length; j++) {
                    if (disponibles[i].cuerda !== disponibles[j].cuerda && Math.abs(disponibles[i].peso - disponibles[j].peso) <= margen) {
                        peleasCasadas.push({ id: contador++, g1: disponibles[i], g2: disponibles[j], ganador: '', min: 0, seg: 0 });
                        disponibles.splice(j, 1); disponibles.splice(i, 1);
                        i--; break;
                    }
                }
            }
        });
        localStorage.setItem('peleas', JSON.stringify(peleasCasadas));
        renderizarTodasPeleas();
        document.getElementById('seccionEstadisticas').style.display = 'block';
    }

    function renderizarTodasPeleas() {
        const cont = document.getElementById('resultadosCotejo');
        cont.innerHTML = "<h2 style='text-align:center; margin: 30px 0;'>⚔️ PROGRAMACIÓN DE COMBATES</h2>";
        peleasCasadas.forEach(p => {
            cont.innerHTML += `
                <div class="match-card">
                    <div class="match-header">
                        <span>COMBATE #${p.id}</span>
                        <span>DIFERENCIA: ${Math.abs(p.g1.peso - p.g2.peso).toFixed(2)} LBS</span>
                    </div>
                    <div class="match-info">
                        <div class="gallo-box" style="text-align:right">
                            <b>${p.g1.cuerda} <small>(F-${p.g1.frente})</small></b>
                            <div class="info-grid">
                                <div class="info-item"><span>Peso</span>${p.g1.peso.toFixed(2)}</div>
                                <div class="info-item"><span>Mes</span>${p.g1.marca}</div>
                                <div class="info-item"><span>Placa</span>${p.g1.placa}</div>
                                <div class="info-item"><span>Anillo</span>${p.g1.anillo}</div>
                            </div>
                        </div>
                        <div class="vs">VS</div>
                        <div class="gallo-box" style="text-align:left">
                            <b>${p.g2.cuerda} <small>(F-${p.g2.frente})</small></b>
                            <div class="info-grid">
                                <div class="info-item"><span>Peso</span>${p.g2.peso.toFixed(2)}</div>
                                <div class="info-item"><span>Mes</span>${p.g2.marca}</div>
                                <div class="info-item"><span>Placa</span>${p.g2.placa}</div>
                                <div class="info-item"><span>Anillo</span>${p.g2.anillo}</div>
                            </div>
                        </div>
                    </div>
                    <div class="result-zone no-print">
                        <div class="time-group">
                            ⏱️ <input type="number" placeholder="Min" value="${p.min || ''}" onchange="guardarTiempo(${p.id}, 'min', this.value)">
                            :
                            <input type="number" placeholder="Seg" value="${p.seg || ''}" onchange="guardarTiempo(${p.id}, 'seg', this.value)">
                        </div>
                        <select onchange="guardarGanador(${p.id}, this.value)" style="width: 200px;">
                            <option value="">Seleccionar Ganador...</option>
                            <option value="g1" ${p.ganador==='g1'?'selected':''}>Gana ${p.g1.cuerda}</option>
                            <option value="g2" ${p.ganador==='g2'?'selected':''}>Gana ${p.g2.cuerda}</option>
                            <option value="T" ${p.ganador==='T'?'selected':''}>Tablas</option>
                        </select>
                    </div>
                </div>`;
        });
    }

    function guardarTiempo(id, tipo, valor) {
        const p = peleasCasadas.find(x => x.id === id);
        p[tipo] = parseInt(valor) || 0;
        localStorage.setItem('peleas', JSON.stringify(peleasCasadas));
    }

    function guardarGanador(id, valor) {
        const p = peleasCasadas.find(x => x.id === id);
        p.ganador = valor;
        localStorage.setItem('peleas', JSON.stringify(peleasCasadas));
    }

    function actualizarEstadisticas() {
        const stats = {};
        gallos.forEach(g => {
            const key = `${g.cuerda} (F-${g.frente})`;
            if(!stats[key]) stats[key] = { inscritos: 0, g: 0, p: 0, t: 0, puntos: 0, totalSeg: 0 };
            stats[key].inscritos++;
        });

        peleasCasadas.forEach(p => {
            if(!p.ganador) return;
            const key1 = `${p.g1.cuerda} (F-${p.g1.frente})`;
            const key2 = `${p.g2.cuerda} (F-${p.g2.frente})`;
            const tPelea = (p.min * 60) + p.seg;
            stats[key1].totalSeg += tPelea; stats[key2].totalSeg += tPelea;

            if(p.ganador === 'g1') { stats[key1].g++; stats[key1].puntos += 3; stats[key2].p++; }
            else if(p.ganador === 'g2') { stats[key2].g++; stats[key2].puntos += 3; stats[key1].p++; }
            else { stats[key1].t++; stats[key1].puntos += 1; stats[key2].t++; stats[key2].puntos += 1; }
        });

        const tbody = document.querySelector("#tablaEstadisticas tbody");
        tbody.innerHTML = Object.keys(stats)
            .sort((a, b) => stats[b].puntos - stats[a].puntos || stats[a].totalSeg - stats[b].totalSeg)
            .map((c, i) => {
                const m = Math.floor(stats[c].totalSeg / 60);
                const s = stats[c].totalSeg % 60;
                return `<tr class="${i === 0 ? 'leader-row' : ''}">
                    <td><b>${c}</b></td><td>${stats[c].inscritos}</td>
                    <td style="color:green">${stats[c].g}</td><td style="color:red">${stats[c].p}</td><td>${stats[c].t}</td>
                    <td><b>${stats[c].puntos} pts</b></td><td>${m}m ${s}s</td>
                </tr>`;
            }).join('');
    }

    function resetearSistema() {
        if(confirm("⚠️ ATENCIÓN: Se borrarán todas las cuerdas, peleas y resultados. ¿Deseas continuar?")) {
            localStorage.removeItem('gallos');
            localStorage.removeItem('peleas');
            location.reload();
        }
    }
</script>
</body>
</html>
