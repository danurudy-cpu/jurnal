# jurnal
treding harian
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<title>Jurnal Trading Profesional</title>
<style>
body {
  font-family: Arial, sans-serif;
  background:#0f172a;
  color:#e5e7eb;
  padding:20px;
}
h1,h2 {
  color:#38bdf8;
}
section {
  background:#020617;
  padding:15px;
  margin-bottom:20px;
  border-radius:10px;
}
label {
  display:block;
  margin-top:10px;
  font-weight:bold;
}
input, textarea, select {
  width:100%;
  padding:8px;
  margin-top:5px;
  background:#020617;
  color:#fff;
  border:1px solid #334155;
  border-radius:5px;
}
button {
  margin-top:15px;
  padding:12px;
  width:100%;
  background:#38bdf8;
  border:none;
  border-radius:8px;
  font-size:16px;
  cursor:pointer;
}
button:hover { background:#0ea5e9; }
.stats {
  display:flex;
  gap:15px;
}
.stats div {
  background:#020617;
  padding:10px;
  border-radius:8px;
  flex:1;
  text-align:center;
}
small { color:#94a3b8; }
</style>
</head>

<body>

<h1>📓 Jurnal Trading Profesional</h1>

<form id="journalForm">

<section>
<h2>1️⃣ Identitas Trade</h2>
<label>Tanggal & Jam Entry</label>
<input type="datetime-local" required>

<label>Pair / Instrumen</label>
<input placeholder="XAUUSD, EURUSD">

<label>Timeframe</label>
<select>
<option>M5</option><option>M15</option><option>H1</option><option>H4</option>
</select>

<label>Session</label>
<select>
<option>Asia</option><option>London</option><option>New York</option>
</select>

<label>Arah Trade</label>
<select>
<option>Buy</option><option>Sell</option>
</select>
</section>

<section>
<h2>2️⃣ Setup & Alasan Entry</h2>
<label>Setup / Strategi</label>
<input placeholder="BOS + Retest">

<label>Alasan Entry</label>
<textarea placeholder="Trend apa, area apa, konfirmasi apa"></textarea>

<label>Alasan TIDAK Entry (jika ragu)</label>
<textarea></textarea>
</section>

<section>
<h2>3️⃣ Risk Management</h2>
<label>Balance Saat Entry</label>
<input type="number">

<label>Lot Size</label>
<input type="number" step="0.01">

<label>Risk per Trade (%)</label>
<input type="number" step="0.1">

<label>Stop Loss (pips / harga)</label>
<input>

<label>Take Profit</label>
<input>

<label>Risk : Reward</label>
<input placeholder="1:2">
</section>

<section>
<h2>4️⃣ Eksekusi Trade</h2>
<label>Entry Sesuai Plan?</label>
<select><option>Ya</option><option>Tidak</option></select>

<label>SL Dipindah? Kenapa?</label>
<textarea></textarea>

<label>Intervensi Manual</label>
<textarea placeholder="Takut / Serakah / Ragu"></textarea>
</section>

<section>
<h2>5️⃣ Hasil Trade</h2>
<label>Profit / Loss ($)</label>
<input type="number">

<label>R Multiple</label>
<input placeholder="+2R / -1R">

<label>Durasi Trade</label>
<input placeholder="30 menit">
</section>

<section>
<h2>6️⃣ Screenshot</h2>
<label>Sebelum Entry</label>
<input type="file">

<label>Setelah Close</label>
<input type="file">
</section>

<section>
<h2>7️⃣ Jurnal Psikologi</h2>
<label>Emosi Sebelum Entry</label>
<textarea></textarea>

<label>Emosi Saat Floating</label>
<textarea></textarea>

<label>Emosi Setelah Close</label>
<textarea></textarea>

<label>Catatan Psikologi</label>
<textarea placeholder="FOMO / Revenge / Overconfidence / Takut Rugi"></textarea>
</section>

<section>
<h2>8️⃣ Evaluasi & Pelajaran</h2>
<label>Apa yang Sudah Benar?</label>
<textarea></textarea>

<label>Kesalahan Utama</label>
<textarea></textarea>

<label>Tidak Boleh Diulang</label>
<textarea></textarea>

<label>Kualitas Setup</label>
<select>
<option>A+ (Ideal)</option>
<option>B (Boleh)</option>
<option>C (Hindari)</option>
</select>
</section>

<button type="submit">💾 Simpan Jurnal</button>
</form>

<section>
<h2>9️⃣ Statistik (Manual Review)</h2>
<div class="stats">
<div>📈 Winrate<br><small>Isi manual</small></div>
<div>📊 Avg R<br><small>Isi manual</small></div>
<div>📉 Max DD<br><small>Isi manual</small></div>
</div>
</section>

<script>
document.getElementById("journalForm").addEventListener("submit", function(e){
  e.preventDefault();
  alert("Jurnal tersimpan. Review sebelum trade berikutnya.");
});
</script>

</body>
</html>
