<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Rajasthan Royal Hindu Marriage Bureau</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root{
  --lux-dark:#111315;
  --lux-card:#1b1e22;
  --lux-gray:#2a2f36;
  --lux-gold:#d4af37;
  --lux-text:#e6e6e6;
}

*{margin:0;padding:0;box-sizing:border-box}
body{
  font-family:'Poppins',sans-serif;
  background:linear-gradient(135deg,#0f1114,#1a1d22);
  color:var(--lux-text);
  overflow-x:hidden;
}

/* ===== NAVBAR ===== */
.navbar{
  position:sticky;top:0;z-index:999;
  backdrop-filter:blur(12px);
  background:rgba(0,0,0,.45);
  border-bottom:1px solid rgba(255,255,255,.08);
  display:flex;justify-content:space-between;align-items:center;
  padding:14px 22px;
}
.logo{
  font-weight:700;
  font-size:20px;
  background:linear-gradient(45deg,var(--lux-gold),#fff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}
.nav-links a{
  color:#ddd;text-decoration:none;margin-left:18px;font-size:14px;
  transition:.3s;
}
.nav-links a:hover{color:var(--lux-gold)}

/* ===== HERO ===== */
.hero{
  min-height:90vh;
  display:flex;align-items:center;justify-content:center;
  text-align:center;padding:40px 20px;
  background:
    radial-gradient(circle at 20% 30%, rgba(212,175,55,.15), transparent 40%),
    radial-gradient(circle at 80% 70%, rgba(255,255,255,.06), transparent 40%),
    linear-gradient(135deg,#0e1013,#1a1d22);
  animation:fadeIn 1.2s ease;
}
.hero h1{
  font-size:42px;margin-bottom:12px;
  background:linear-gradient(45deg,#fff,var(--lux-gold));
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}
.hero p{opacity:.85}

.btn{
  display:inline-block;margin-top:22px;
  padding:12px 26px;border-radius:12px;
  background:linear-gradient(45deg,var(--lux-gold),#b8962e);
  color:#000;text-decoration:none;font-weight:600;
  transition:.35s;
  box-shadow:0 10px 25px rgba(212,175,55,.35);
}
.btn:hover{
  transform:translateY(-3px) scale(1.04);
  box-shadow:0 18px 40px rgba(212,175,55,.45);
}

/* ===== SECTIONS ===== */
section{max-width:1250px;margin:auto;padding:70px 18px}
.section-title{
  text-align:center;margin-bottom:35px;font-size:28px;
  background:linear-gradient(45deg,#fff,var(--lux-gold));
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

/* ===== FILTER ===== */
.filters{text-align:center;margin-bottom:28px}
select{
  padding:10px 12px;margin:6px;border-radius:10px;
  background:var(--lux-gray);color:#fff;border:1px solid #444;
}

/* ===== CARDS ===== */
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
  gap:22px;
}
.card{
  background:linear-gradient(145deg,#1b1e22,#111315);
  border:1px solid rgba(255,255,255,.05);
  border-radius:22px;
  padding:16px;
  text-align:center;
  transition:.45s;
  position:relative;
  overflow:hidden;
}
.card::before{
  content:"";
  position:absolute;inset:0;
  background:linear-gradient(120deg,transparent,rgba(212,175,55,.18),transparent);
  opacity:0;transition:.5s;
}
.card:hover::before{opacity:1}
.card:hover{
  transform:translateY(-8px) scale(1.02);
  box-shadow:0 25px 60px rgba(0,0,0,.6);
}
.card img{
  width:100%;height:240px;object-fit:cover;
  border-radius:14px;margin-bottom:10px;
}
.tag{font-size:13px;color:#bbb;margin:2px 0}

/* ===== FORM BOX ===== */
.form-box{
  background:linear-gradient(145deg,#1b1e22,#111315);
  border:1px solid rgba(255,255,255,.06);
  padding:22px;border-radius:22px;
  box-shadow:0 20px 50px rgba(0,0,0,.5);
}

/* ===== FOOTER ===== */
footer{
  text-align:center;padding:28px;
  background:#0b0c0f;
  border-top:1px solid rgba(255,255,255,.06);
}

/* ===== FLOAT WA ===== */
.wa-float{
  position:fixed;right:20px;bottom:20px;
  background:#25d366;color:#fff;
  padding:16px;border-radius:50%;
  font-size:22px;text-decoration:none;
  box-shadow:0 12px 30px rgba(0,0,0,.6);
  animation:float 2.6s infinite ease-in-out;
}

@keyframes float{
  0%,100%{transform:translateY(0)}
  50%{transform:translateY(-8px)}
}
@keyframes fadeIn{
  from{opacity:0;transform:translateY(30px)}
  to{opacity:1;transform:none}
}
</style>
</head>
<body>

<div class="navbar">
  <div class="logo">💍 Rajasthan Royal Hindu Marriage Bureau</div>
  <div class="nav-links">
    <a href="#home">Home</a>
    <a href="#profiles">Profiles</a>
    <a href="#register">Register</a>
    <a href="#contact">Contact</a>
  </div>
</div>

<div id="home" class="hero">
  <div>
    <h1>Find Your Perfect Life Partner</h1>
    <p>Premium Verified Hindu Matrimony Service</p>
    <a href="#register" class="btn">Register Now</a>
  </div>
</div>

<section id="profiles">
  <h2 class="section-title">Latest Profiles</h2>

  <div class="filters">
    <select id="casteFilter"><option value="">All Caste</option></select>
    <select id="ageFilter">
      <option value="">Max Age</option>
      <option value="25">25</option>
      <option value="30">30</option>
      <option value="35">35</option>
      <option value="40">40</option>
    </select>
  </div>

  <div id="profilesGrid" class="grid"></div>
</section>

<section id="register">
  <h2 class="section-title">Register Profile</h2>
  <div class="form-box">
    <p style="text-align:center;margin-bottom:12px">
      Registration Fee: <b>Ladka ₹1000 | Ladki ₹500</b>
    </p>

    <!-- ✅ APNA GOOGLE FORM LINK YAHAN PASTE KAR -->
    <iframe src="PASTE_YOUR_GOOGLE_FORM_LINK_HERE" width="100%" height="620" frameborder="0"></iframe>
  </div>
</section>

<section id="contact">
  <h2 class="section-title">Contact Us</h2>
  <div class="form-box" style="text-align:center">
    <p><b>Phone/WhatsApp:</b> 8619776286</p>
    <p><b>Location:</b> Rajasthan, India</p>
    <a class="btn" href="https://wa.me/918619776286" target="_blank">Chat on WhatsApp</a>
  </div>
</section>

<footer>
  © 2026 Rajasthan Royal Hindu Marriage Bureau
</footer>

<a class="wa-float" href="https://wa.me/918619776286" target="_blank">💬</a>

<script>
const SHEET_ID="PASTE_YOUR_GOOGLE_SHEET_ID";
const SHEET_NAME="Approved";
const url=`https://opensheet.elk.sh/${SHEET_ID}/${SHEET_NAME}`;

const grid=document.getElementById("profilesGrid");
const casteFilter=document.getElementById("casteFilter");
const ageFilter=document.getElementById("ageFilter");
let allData=[];

function driveToDirect(u){
  if(!u) return "https://via.placeholder.com/300x300?text=No+Photo";
  const m=u.match(/[-\\w]{25,}/);
  return m?`https://drive.google.com/uc?export=view&id=${m[0]}`:u;
}

function render(data){
  grid.innerHTML="";
  data.forEach(p=>{
    grid.innerHTML+=`
      <div class="card">
        <img src="${driveToDirect(p.Photo)}">
        <h3>${p.Name||"Profile"}</h3>
        <div class="tag">Age: ${p.Age||"-"}</div>
        <div class="tag">Height: ${p.Height||"-"}</div>
        <div class="tag">Education: ${p.Education||"-"}</div>
        <div class="tag">Job: ${p.Job||"-"}</div>
        <div class="tag">Caste: ${p.Caste||"-"}</div>
      </div>`;
  });
}

function applyFilter(){
  let filtered=[...allData];
  if(casteFilter.value) filtered=filtered.filter(x=>x.Caste===casteFilter.value);
  if(ageFilter.value) filtered=filtered.filter(x=>Number(x.Age)<=Number(ageFilter.value));
  render(filtered);
}

casteFilter.onchange=applyFilter;
ageFilter.onchange=applyFilter;

fetch(url)
  .then(r=>r.json())
  .then(data=>{
    allData=data;
    render(allData);
    const castes=[...new Set(data.map(x=>x.Caste).filter(Boolean))];
    castes.forEach(c=>{
      casteFilter.innerHTML+=`<option value="${c}">${c}</option>`;
    });
  })
  .catch(()=>{
    grid.innerHTML="<p style='text-align:center'>Profiles loading soon...</p>";
  });
</script>

</body>
