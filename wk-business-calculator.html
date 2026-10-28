<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>WK Business Calculator</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;700;800&display=swap">
<style>
:root{--bg:#fff;--sf:#F6F9FA;--ink:#1e344b;--mu:#5E7186;--ln:#DCE4EA;--ac:#40c4ad;--on:#1e344b;--ring:#1e344b;--hero:#1e344b;--gold:#40c4ad;--bad:#C0392B;--ok:#13806C;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);color-scheme:light}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0F1B28;--sf:#162636;--ink:#E8EEF3;--mu:#9DB0C2;--ln:#27384A;--ring:#40c4ad;--hero:#1e344b;--bad:#F07B6B;--ok:#40c4ad;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#0F1B28;--sf:#162636;--ink:#E8EEF3;--mu:#9DB0C2;--ln:#27384A;--ring:#40c4ad;--hero:#1e344b;--bad:#F07B6B;--ok:#40c4ad;color-scheme:dark}
*{box-sizing:inherit}
body{margin:0;background:var(--bg);color:var(--ink);font:400 15px/1.5 "Plus Jakarta Sans",system-ui,-apple-system,"Segoe UI",sans-serif;font-variant-numeric:tabular-nums}
.wrap{max-width:1080px;margin:0 auto;padding:20px 16px 48px}
header{display:flex;justify-content:space-between;align-items:end;gap:12px;flex-wrap:wrap;margin-bottom:18px}
h1{margin:0;font-size:clamp(26px,5vw,38px);font-weight:800;letter-spacing:-.02em;line-height:1.1}
header p{margin:6px 0 0;color:var(--mu);max-width:48ch}
.seg{display:inline-flex;background:var(--sf);border:1px solid var(--ln);border-radius:10px;padding:3px}
.seg button{border:0;background:none;color:var(--mu);font:inherit;font-weight:700;padding:7px 14px;border-radius:8px;cursor:pointer}
.seg button[aria-pressed="true"]{background:var(--ac);color:var(--on)}
.seg button:focus-visible,input:focus-visible{outline:2px solid var(--ring);outline-offset:2px}
.grid{display:grid;grid-template-columns:minmax(0,1fr) minmax(0,1.1fr);gap:20px;align-items:start}
@media(max-width:820px){.grid{grid-template-columns:1fr}}
fieldset{background:var(--sf);border:1px solid var(--ln);border-radius:12px;margin:0 0 14px;padding:6px 16px 10px;min-width:0}
legend{font-weight:800;font-size:15px;padding:0 6px;margin-left:-6px}
.row{display:flex;justify-content:space-between;align-items:center;gap:12px;padding:6px 0;border-bottom:1px solid var(--ln)}
.row:last-child{border-bottom:0}
.row label{flex:1;font-size:14px}
.f{display:flex;align-items:center;gap:6px;background:var(--bg);border:1px solid var(--ln);border-radius:8px;padding:0 8px;width:170px}
.f span{color:var(--mu);font-size:13px}
.f input{width:100%;min-width:0;border:0;background:none;color:var(--ink);font:inherit;text-align:right;padding:7px 0}
.sum{display:flex;justify-content:space-between;font-weight:700;padding-top:8px;color:var(--mu)}
.res{position:sticky;top:12px}
@media(max-width:820px){.res{position:static}}
.hero{background:var(--hero);color:#E6F0ED;border-radius:14px;padding:22px 20px;margin-bottom:14px}
.hero small{display:block;opacity:.75;font-size:14px}
.hero b{display:block;font-size:clamp(34px,8vw,54px);line-height:1.05;font-weight:800;color:var(--gold);margin:4px 0}
.hero.neg b{color:#FF9D8F}
.m{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:10px;margin-bottom:14px}
.m div{background:var(--sf);border:1px solid var(--ln);border-radius:10px;padding:10px 12px}
.m small{color:var(--mu);display:block;font-size:12.5px}
.m strong{font-size:18px;font-weight:800}
.pos{color:var(--ok)}.neg{color:var(--bad)}
.card{background:var(--sf);border:1px solid var(--ln);border-radius:12px;padding:14px 16px;margin-bottom:14px}
.card h2{margin:0 0 6px;font-size:15px}
svg{width:100%;height:auto;display:block}
.warn{margin:0;padding-left:18px;color:var(--bad);font-size:14px}
.note{color:var(--mu);font-size:13px;margin:0}
</style>
</head>
<body>
<div class="wrap">
<header>
<div>
<h1>WK Business Calculator</h1>
<p>Isi angka usahamu, lihat kapan balik modal dan berapa laba per bulan. Semua hitungan berjalan otomatis.</p>
</div>
<div class="seg" role="group" aria-label="Skenario penjualan" id="scn">
<button data-m="0.7" aria-pressed="false">Pesimis −30%</button>
<button data-m="1" aria-pressed="true">Realistis</button>
<button data-m="1.3" aria-pressed="false">Optimis +30%</button>
</div>
</header>
<div class="grid">
<form id="inp" onsubmit="return false"></form>
<section class="res" aria-live="polite">
<div class="hero" id="hero"></div>
<div class="m" id="mets"></div>
<div class="card"><h2>Arus kas kumulatif</h2><div id="chart"></div><p class="note" id="cnote"></p></div>
<div class="card" id="wcard"><h2>Catatan</h2><ul class="warn" id="warn"></ul></div>
</section>
</div>
</div>
<script>
var G=[
["Modal awal (sekali bayar)","modal",[["peralatan","Peralatan / mesin",15e6,"Rp"],["renov","Renovasi, sewa di muka, deposit",10e6,"Rp"],["izin","Perizinan & legalitas",1e6,"Rp"],["stok","Stok awal",3e6,"Rp"],["promo","Branding & promosi pembukaan",2e6,"Rp"],["cad","Dana cadangan",3e6,"Rp"]]],
["Penjualan","jual",[["harga","Harga jual per unit",20000,"Rp"],["perhari","Terjual per hari",55,"unit"],["hari","Hari buka per bulan",26,"hari"],["tumbuh","Pertumbuhan penjualan per bulan",0,"%"]]],
["COGS / HPP per unit","cogs",[["bahan","Bahan baku",6000,"Rp"],["kemasan","Kemasan",1500,"Rp"],["produksi","Biaya produksi langsung",500,"Rp"],["waste","Waste (rusak / tidak laku)",5,"%"],["komisi","Komisi platform & pembayaran",0,"%"]]],
["Biaya tetap per bulan","tetap",[["sewa","Sewa tempat",3e6,"Rp"],["gaji","Gaji karyawan",4e6,"Rp"],["listrik","Listrik, air, internet",6e5,"Rp"],["mkt","Marketing / iklan",5e5,"Rp"],["cicil","Cicilan / bunga pinjaman",0,"Rp"],["lain","Lain-lain",4e5,"Rp"],["pemilik","Gaji pemilik",3e6,"Rp"]]],
["Pajak","pajak",[["pajak","Pajak dari omzet (PPh final UMKM 0,5%)",0.5,"%"]]]
];
var mult=1,$=function(i){return document.getElementById(i)};
var form=$("inp");
G.forEach(function(g){
var fs=document.createElement("fieldset"),h='<legend>'+g[0]+'</legend>';
g[2].forEach(function(f){
var pre=f[3]==="Rp"?'<span>Rp</span>':'',suf=f[3]!=="Rp"?'<span>'+f[3]+'</span>':'';
h+='<div class="row"><label for="'+f[0]+'">'+f[1]+'</label><div class="f">'+pre+'<input id="'+f[0]+'" data-g="'+g[1]+'" type="number" inputmode="decimal" min="0" step="any" value="'+f[2]+'">'+suf+'</div></div>';
});
if(g[1]==="modal"||g[1]==="tetap")h+='<div class="sum"><span>Total</span><span id="sum_'+g[1]+'"></span></div>';
fs.innerHTML=h;form.appendChild(fs);
});
function v(i){return Math.max(0,parseFloat($(i).value)||0)}
function rp(n){var a=Math.abs(n),s=n<0?"−":"";
if(a>=1e9)return s+"Rp "+(a/1e9).toLocaleString("id-ID",{maximumFractionDigits:2})+" miliar";
if(a>=1e6)return s+"Rp "+(a/1e6).toLocaleString("id-ID",{maximumFractionDigits:1})+" juta";
return s+"Rp "+Math.round(a).toLocaleString("id-ID")}
function num(n,d){return n.toLocaleString("id-ID",{maximumFractionDigits:d==null?1:d})}
function calc(){
var modal=0,tetap=0;
["peralatan","renov","izin","stok","promo","cad"].forEach(function(i){modal+=v(i)});
["sewa","gaji","listrik","mkt","cicil","lain","pemilik"].forEach(function(i){tetap+=v(i)});
$("sum_modal").textContent=rp(modal);$("sum_tetap").textContent=rp(tetap);
var harga=v("harga"),u0=v("perhari")*v("hari")*mult,g=v("tumbuh")/100,tax=v("pajak")/100;
var cu=(v("bahan")+v("kemasan")+v("produksi"))*(1+v("waste")/100)+harga*v("komisi")/100;
var contrib=harga-cu-harga*tax;
var cum=[-modal],pay=null,net1=0,m;
for(m=1;m<=60;m++){
var u=u0*Math.pow(1+g,m-1),net=u*contrib-tetap;
if(m===1)net1=net;
var prev=cum[m-1];cum.push(prev+net);
if(pay===null&&prev<0&&prev+net>=0)pay=(m-1)+(-prev)/net;
}
if(modal===0)pay=0;
var omzet=u0*harga,cogs=u0*cu,gross=omzet-cogs,taxv=omzet*tax;
var bep=contrib>0?tetap/contrib:null;
render({modal:modal,tetap:tetap,harga:harga,u0:u0,cu:cu,omzet:omzet,cogs:cogs,gross:gross,taxv:taxv,net:net1,pay:pay,bep:bep,cum:cum,contrib:contrib});
}
function render(r){
var hero=$("hero"),bad=r.pay===null;
hero.className="hero"+(bad?" neg":"");
hero.innerHTML=bad?'<small>Balik modal</small><b>Belum dalam 5 tahun</b><small>Dengan angka ini, arus kas kumulatif belum menutup modal sampai bulan ke-60.</small>'
:'<small>Balik modal dalam</small><b>'+(r.pay===0?"Langsung":num(r.pay)+" bulan")+'</b><small>Laba bersih bulan pertama '+rp(r.net)+'</small>';
var gm=r.omzet>0?r.gross/r.omzet*100:0,nm=r.omzet>0?r.net/r.omzet*100:0;
var bepTxt=r.bep===null?"–":num(Math.ceil(r.bep),0)+" unit";
var items=[["Omzet / bulan",rp(r.omzet)],["COGS per unit",rp(r.cu)],["Total COGS / bulan",rp(r.cogs)],["Laba kotor · margin",rp(r.gross)+" · "+num(gm)+"%"],
["Laba bersih / bulan",'<span class="'+(r.net>=0?"pos":"neg")+'">'+rp(r.net)+"</span>"],["Net margin",num(nm)+"%"],
["Titik impas (BEP)",bepTxt+" / bulan"],["Terjual sekarang",num(r.u0,0)+" unit / bulan"]];
$("mets").innerHTML=items.map(function(x){return"<div><small>"+x[0]+"</small><strong>"+x[1]+"</strong></div>"}).join("");
chart(r);
var w=[];
if(r.harga>0&&r.harga<=r.cu)w.push("Harga jual lebih rendah dari COGS per unit. Setiap penjualan menambah rugi.");
else if(r.contrib<=0)w.push("Setelah pajak, margin per unit tidak positif.");
if(r.net<0)w.push("Laba bersih bulanan negatif. Naikkan harga, kurangi biaya, atau tambah volume.");
if(r.pay!==null&&r.pay>24)w.push("Balik modal lebih dari 24 bulan. Risiko tinggi untuk usaha kecil.");
if(r.bep!==null&&r.u0<r.bep&&r.net<0)w.push("Penjualan ("+num(r.u0,0)+" unit) di bawah titik impas ("+num(Math.ceil(r.bep),0)+" unit).");
if(!w.length)w.push("Tidak ada peringatan. Coba skenario pesimis untuk menguji ketahanan usahamu.");
$("warn").innerHTML=w.map(function(x){return"<li>"+x+"</li>"}).join("");
$("warn").style.color=w.length===1&&w[0].indexOf("Tidak ada")===0?"var(--mu)":"var(--bad)";
}
function chart(r){
var N=r.pay!==null?Math.min(60,Math.max(12,Math.ceil(r.pay*1.6))):24,d=r.cum.slice(0,N+1);
var W=600,H=250,L=8,R=8,T=14,B=26,mn=Math.min.apply(null,d.concat(0)),mx=Math.max.apply(null,d.concat(0));
if(mx===mn){mx=mn+1}
var X=function(i){return L+i/N*(W-L-R)},Y=function(y){return T+(mx-y)/(mx-mn)*(H-T-B)};
var pts=d.map(function(y,i){return X(i).toFixed(1)+","+Y(y).toFixed(1)}).join(" ");
var z=Y(0).toFixed(1),s='<svg viewBox="0 0 '+W+' '+H+'" role="img" aria-label="Grafik arus kas kumulatif per bulan">';
s+='<line x1="'+L+'" x2="'+(W-R)+'" y1="'+z+'" y2="'+z+'" stroke="var(--mu)" stroke-dasharray="4 4"/>';
s+='<polyline points="'+pts+'" fill="none" stroke="var(--ring)" stroke-width="3" stroke-linejoin="round"/>';
if(r.pay!==null&&r.pay<=N&&r.pay>0)s+='<circle cx="'+X(r.pay).toFixed(1)+'" cy="'+z+'" r="6" fill="var(--gold)" stroke="var(--ink)" stroke-width="2"/>';
var st=Math.max(1,Math.round(N/6));
for(var i=0;i<=N;i+=st)s+='<text x="'+X(i).toFixed(1)+'" y="'+(H-8)+'" font-size="12" fill="var(--mu)" text-anchor="middle">'+i+'</text>';
$("chart").innerHTML=s+'</svg>';
$("cnote").textContent="Sumbu bawah: bulan. Garis putus-putus adalah titik nol; titik kuning menandai balik modal. Garis dimulai dari −"+rp(r.modal).replace("−","")+" (modal awal).";
}
form.addEventListener("input",calc);
$("scn").addEventListener("click",function(e){
var b=e.target.closest("button");if(!b)return;
mult=parseFloat(b.dataset.m);
[].forEach.call($("scn").children,function(x){x.setAttribute("aria-pressed",x===b)});
calc();
});
calc();
</script>
</body>
</html>
