---
title: "Second post"
description: "Lorem ipsum dolor sit amet"
pubDate: "Jul 15 2022"
heroImage: "/blog-placeholder-4.jpg"
---

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@400;600;700&family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
<style>
/* ============================================
   KEYFRAME ANIMATIONS
============================================ */
@keyframes gradientShift {
  0%   { background-position: 0% 50%; }
  50%  { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

@keyframes floatUp {
  0%, 100% { transform: translateY(0px); }
  50%       { transform: translateY(-8px); }
}

@keyframes glowPulse {
  0%, 100% { box-shadow: 0 0 20px rgba(255, 0, 0, 0.2), 0 0 40px rgba(200, 0, 0, 0.1); }
  50%       { box-shadow: 0 0 40px rgba(255, 215, 0, 0.7), 0 0 80px rgba(255, 150, 0, 0.3); }
}

@keyframes numberPulse {
  0%, 100% { transform: scale(1); box-shadow: 0 0 15px rgba(255, 215, 0, 0.5); }
  50%       { transform: scale(1.1); box-shadow: 0 0 30px rgba(255, 215, 0, 0.9); }
}

@keyframes lineExpand {
  from { width: 0; }
  to   { width: 80px; }
}

@keyframes shimmer {
  0%   { background-position: -200% center; }
  100% { background-position: 200% center; }
}

@keyframes borderRotate {
  0%   { background-position: 0% 50%; }
  100% { background-position: 400% 50%; }
}

@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(40px); }
  to   { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInLeft {
  from { opacity: 0; transform: translateX(-40px); }
  to   { opacity: 1; transform: translateX(0); }
}

@keyframes scanLine {
  0%   { transform: translateY(-100%); opacity: 0.5; }
  100% { transform: translateY(100vh); opacity: 0; }
}

@keyframes particleDrift {
  0%   { transform: translateY(0) translateX(0) rotate(0deg); opacity: 1; }
  100% { transform: translateY(-100px) translateX(30px) rotate(360deg); opacity: 0; }
}

@keyframes tableRowGlow {
  0%, 100% { background: rgba(255, 255, 255, 0.02); }
  50%       { background: rgba(255, 215, 0, 0.05); }
}

@keyframes countdownBlink {
  0%, 100% { opacity: 1; }
  50%       { opacity: 0.5; }
}

@keyframes iconSpin {
  from { transform: rotate(0deg); }
  to   { transform: rotate(360deg); }
}

@keyframes progressFill {
  from { width: 0%; }
  to   { width: 100%; }
}

@keyframes titleGlow {
  0%, 100% {
    text-shadow:
      0 0 10px rgba(255, 215, 0, 0.5),
      0 0 20px rgba(255, 150, 0, 0.3),
      0 2px 4px rgba(0,0,0,0.5);
  }
  50% {
    text-shadow:
      0 0 20px rgba(255, 215, 0, 1),
      0 0 40px rgba(255, 150, 0, 0.6),
      0 0 60px rgba(255, 100, 0, 0.3),
      0 2px 4px rgba(0,0,0,0.5);
  }
}

@keyframes stepConnector {
  0%, 100% { opacity: 0.3; }
  50%       { opacity: 1; }
}

/* ============================================
   SECTION CARA DAFTAR
============================================ */
.cara-daftar {
  position: relative;
  padding: 80px 20px 100px;
  background:
    radial-gradient(ellipse at 20% 50%, rgba(255, 0, 0, 0.12) 0%, transparent 60%),
    radial-gradient(ellipse at 80% 20%, rgba(200, 0, 0, 0.1) 0%, transparent 50%),
    radial-gradient(ellipse at 50% 100%, rgba(255, 0, 0, 0.08) 0%, transparent 60%),
    linear-gradient(160deg, #180202 0%, #200505 30%, #180303 60%, #100101 100%);
  color: #ffffff;
  text-align: center;
  overflow: hidden;
}

/* Grid background pattern */
.cara-daftar::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(255, 0, 0, 0.025) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255, 0, 0, 0.025) 1px, transparent 1px);
  background-size: 50px 50px;
  pointer-events: none;
}

/* Scan line dekorasi */
.cara-daftar::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    #ffd700 20%,
    #ffffff 50%,
    #ffd700 80%,
    transparent 100%
  );
  background-size: 200% 100%;
  animation: borderRotate 4s linear infinite;
}

/* ============================================
   SECTION TITLE
============================================ */
.section-title-wrap {
  position: relative;
  margin-bottom: 60px;
  animation: fadeInUp 0.8s ease-out both;
}

.section-badge {
  display: inline-block;
  padding: 6px 20px;
  background: linear-gradient(135deg, rgba(255, 215, 0, 0.15), rgba(200, 0, 0, 0.1));
  border: 1px solid rgba(255, 0, 0, 0.2);
  border-radius: 50px;
  font-family: 'Orbitron', sans-serif;
  font-size: 11px;
  font-weight: 700;
  letter-spacing: 3px;
  color: #ffd700;
  text-transform: uppercase;
  margin-bottom: 16px;
  backdrop-filter: blur(10px);
}

.cara-daftar h2,
.situs-judi h2 {
  font-family: 'Orbitron', sans-serif;
  font-size: 38px;
  font-weight: 900;
  margin-bottom: 16px;
  background: linear-gradient(
    135deg,
    #ffffff 0%,
    #ffd700 30%,
    #ffec6e 50%,
    #ffd700 70%,
    #ff8c00 100%
  );
  background-size: 200% auto;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  animation: shimmer 4s linear infinite, titleGlow 3s ease-in-out infinite;
  line-height: 1.2;
}

/* Garis dekorasi bawah judul */
.title-underline {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  margin-top: 12px;
}

.title-underline span {
  height: 2px;
  border-radius: 2px;
  background: linear-gradient(90deg, transparent, #ffd700, transparent);
  animation: lineExpand 1s ease-out 0.5s both;
}

.title-underline span:nth-child(1) { width: 60px; }
.title-underline span:nth-child(3) { width: 60px; }

.title-underline-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #ffd700;
  box-shadow: 0 0 10px #ffd700;
  animation: glowPulse 2s ease-in-out infinite;
}

/* ============================================
   INTRO TEXT
============================================ */
.cara-daftar-intro {
  font-family: 'Inter', sans-serif;
  font-size: 17px;
  max-width: 700px;
  margin: 0 auto 50px;
  line-height: 1.8;
  color: rgba(255, 255, 255, 0.7);
  animation: fadeInUp 0.8s ease-out 0.2s both;
}

/* ============================================
   STEPS CONTAINER
============================================ */
.steps-container {
  max-width: 860px;
  margin: 0 auto 50px;
  display: flex;
  flex-direction: column;
  gap: 0;
  position: relative;
}

/* Garis vertikal penghubung */
.steps-container::before {
  content: '';
  position: absolute;
  left: 34px;
  top: 35px;
  bottom: 35px;
  width: 2px;
  background: linear-gradient(
    180deg,
    transparent 0%,
    rgba(255, 215, 0, 0.4) 10%,
    rgba(255, 215, 0, 0.4) 90%,
    transparent 100%
  );
  animation: stepConnector 3s ease-in-out infinite;
}

/* ============================================
   STEP ITEM
============================================ */
.step-item {
  display: flex;
  align-items: flex-start;
  gap: 20px;
  padding: 20px 24px;
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.06);
  border-radius: 16px;
  margin-bottom: 12px;
  position: relative;
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  backdrop-filter: blur(10px);
  text-align: left;
  animation: fadeInLeft 0.6s ease-out both;
  overflow: hidden;
}

.step-item:nth-child(1) { animation-delay: 0.1s; }
.step-item:nth-child(2) { animation-delay: 0.2s; }
.step-item:nth-child(3) { animation-delay: 0.3s; }
.step-item:nth-child(4) { animation-delay: 0.4s; }
.step-item:nth-child(5) { animation-delay: 0.5s; }

/* Hover shimmer effect */
.step-item::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    90deg,
    transparent 0%,
    rgba(255, 215, 0, 0.05) 50%,
    transparent 100%
  );
  transition: left 0.5s ease;
}

.step-item:hover::before {
  left: 100%;
}

.step-item:hover {
  background: rgba(255, 215, 0, 0.06);
  border-color: rgba(255, 215, 0, 0.25);
  transform: translateX(8px);
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.3),
    0 0 0 1px rgba(255, 215, 0, 0.1),
    inset 0 1px 0 rgba(255, 255, 255, 0.05);
}

/* Left accent bar */
.step-item::after {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 3px;
  background: linear-gradient(180deg, #ffd700, #ff8c00);
  border-radius: 3px 0 0 3px;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.step-item:hover::after {
  opacity: 1;
}

/* ============================================
   STEP NUMBER
============================================ */
.step-number {
  flex-shrink: 0;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Orbitron', sans-serif;
  font-size: 18px;
  font-weight: 900;
  position: relative;
  z-index: 2;

  background: linear-gradient(
    145deg,
    #1a1a2e 0%,
    #16213e 100%
  );
  border: 2px solid rgba(255, 215, 0, 0.4);
  color: #ffd700;
  box-shadow:
    0 0 15px rgba(255, 0, 0, 0.2),
    inset 0 1px 0 rgba(255, 255, 255, 0.1);
  transition: all 0.3s ease;
}

.step-item:hover .step-number {
  background: linear-gradient(145deg, #ffd700 0%, #ff8c00 100%);
  color: #000;
  border-color: #ffd700;
  animation: numberPulse 1.5s ease-in-out infinite;
}

/* ============================================
   STEP CONTENT
============================================ */
.step-content {
  flex: 1;
  padding-top: 4px;
}

.step-title {
  font-family: 'Rajdhani', sans-serif;
  font-size: 18px;
  font-weight: 700;
  color: #ffffff;
  margin-bottom: 4px;
  letter-spacing: 0.5px;
  transition: color 0.3s ease;
}

.step-item:hover .step-title {
  color: #ffd700;
}

.step-desc {
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  color: rgba(255, 255, 255, 0.5);
  line-height: 1.6;
}

/* Step icon kanan */
.step-icon {
  flex-shrink: 0;
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 20px;
  opacity: 0.4;
  transition: all 0.3s ease;
  filter: grayscale(1);
}

.step-item:hover .step-icon {
  opacity: 1;
  filter: grayscale(0);
  animation: floatUp 2s ease-in-out infinite;
}

/* ============================================
   OUTRO TEXT
============================================ */
.cara-daftar-outro {
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  max-width: 600px;
  margin: 0 auto 40px;
  color: rgba(255, 255, 255, 0.6);
  line-height: 1.8;
  animation: fadeInUp 0.8s ease-out 0.6s both;
}

/* ============================================
   CTA BUTTON
============================================ */
.cta-wrap {
  animation: fadeInUp 0.8s ease-out 0.8s both;
}

.cta-daftar {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 16px 48px;
  font-family: 'Orbitron', sans-serif;
  font-size: 14px;
  font-weight: 700;
  letter-spacing: 2px;
  text-decoration: none;
  color: #000;
  position: relative;
  border-radius: 50px;
  overflow: hidden;
  transition: all 0.3s ease;

  background: linear-gradient(
    135deg,
    #ff8c00 0%,
    #ffd700 30%,
    #ffec6e 50%,
    #ffd700 70%,
    #ff8c00 100%
  );
  background-size: 200% auto;
  box-shadow:
    0 0 20px rgba(255, 215, 0, 0.4),
    0 8px 25px rgba(255, 150, 0, 0.3),
    inset 0 1px 0 rgba(255, 255, 255, 0.4);
  animation: shimmer 3s linear infinite;
}

.cta-daftar::before {
  content: '';
  position: absolute;
  inset: 2px;
  border-radius: 48px;
  background: linear-gradient(
    135deg,
    rgba(255,255,255,0.2) 0%,
    transparent 50%
  );
  pointer-events: none;
}

.cta-daftar:hover {
  transform: translateY(-3px) scale(1.03);
  box-shadow:
    0 0 40px rgba(255, 215, 0, 0.7),
    0 15px 35px rgba(255, 150, 0, 0.5),
    inset 0 1px 0 rgba(255, 255, 255, 0.5);
}

.cta-daftar span {
  position: relative;
  z-index: 1;
}

.cta-arrow {
  font-size: 18px;
  transition: transform 0.3s ease;
}

.cta-daftar:hover .cta-arrow {
  transform: translateX(5px);
}

/* ============================================
   FLOATING PARTICLES DEKORASI
============================================ */
.particle-wrap {
  position: absolute;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
}

.particle {
  position: absolute;
  border-radius: 50%;
  background: rgba(255, 215, 0, 0.15);
  animation: particleDrift linear infinite;
}

.particle:nth-child(1)  { width:6px;  height:6px;  left:10%; bottom:20%; animation-duration:8s;  animation-delay:0s;   }
.particle:nth-child(2)  { width:4px;  height:4px;  left:25%; bottom:10%; animation-duration:10s; animation-delay:1s;   }
.particle:nth-child(3)  { width:8px;  height:8px;  left:40%; bottom:30%; animation-duration:7s;  animation-delay:2s;   }
.particle:nth-child(4)  { width:3px;  height:3px;  left:60%; bottom:15%; animation-duration:12s; animation-delay:0.5s; }
.particle:nth-child(5)  { width:5px;  height:5px;  left:75%; bottom:25%; animation-duration:9s;  animation-delay:1.5s; }
.particle:nth-child(6)  { width:7px;  height:7px;  left:88%; bottom:10%; animation-duration:11s; animation-delay:3s;   }
.particle:nth-child(7)  { width:4px;  height:4px;  left:15%; bottom:50%; animation-duration:6s;  animation-delay:2.5s; }
.particle:nth-child(8)  { width:6px;  height:6px;  left:50%; bottom:60%; animation-duration:14s; animation-delay:0.8s; }

/* ============================================
   SECTION BANDAR SLOT
============================================ */
.situs-judi {
  position: relative;
  padding: 80px 20px 100px;
  background:
    radial-gradient(ellipse at 80% 50%, rgba(200, 0, 0, 0.1) 0%, transparent 60%),
    radial-gradient(ellipse at 20% 80%, rgba(255, 0, 0, 0.08) 0%, transparent 50%),
    linear-gradient(160deg, #180202 0%, #200505 30%, #180303 60%, #100101 100%);
  color: #ffffff;
  text-align: center;
  overflow: hidden;
}

.situs-judi::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(255, 0, 0, 0.025) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255, 0, 0, 0.025) 1px, transparent 1px);
  background-size: 50px 50px;
  pointer-events: none;
}

.situs-judi::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    #00e1ff 20%,
    #ffffff 50%,
    #00e1ff 80%,
    transparent 100%
  );
  background-size: 200% 100%;
  animation: borderRotate 4s linear infinite;
}

/* ============================================
   TABLE WRAPPER
============================================ */
.table-wrapper {
  max-width: 960px;
  margin: 0 auto;
  position: relative;
  animation: fadeInUp 0.8s ease-out 0.3s both;
}

/* Border animasi di sekeliling tabel */
.table-border-glow {
  position: relative;
  border-radius: 20px;
  padding: 2px;
  background: linear-gradient(
    135deg,
    rgba(255, 215, 0, 0.6) 0%,
    rgba(0, 200, 255, 0.4) 25%,
    rgba(255, 150, 0, 0.6) 50%,
    rgba(0, 200, 255, 0.4) 75%,
    rgba(255, 215, 0, 0.6) 100%
  );
  background-size: 400% 400%;
  animation: borderRotate 4s linear infinite;
  box-shadow:
    0 0 30px rgba(255, 215, 0, 0.2),
    0 0 60px rgba(255, 0, 0, 0.08);
}

/* ============================================
   PASARAN TABLE
============================================ */
.pasaran-table {
  width: 100%;
  border-collapse: collapse;
  border-radius: 18px;
  overflow: hidden;
}

/* TABLE HEADER */
.pasaran-table thead tr {
  background: linear-gradient(
    135deg,
    #1a1200 0%,
    #2a1f00 30%,
    #1a1200 100%
  );
  position: relative;
}

.pasaran-table th {
  padding: 20px 24px;
  text-align: center;
  font-family: 'Orbitron', sans-serif;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #ffd700;
  border-bottom: 1px solid rgba(255, 215, 0, 0.2);
  position: relative;
}

.pasaran-table th::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 10%;
  right: 10%;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(255,215,0,0.5), transparent);
}

/* Ikon di header */
.th-icon {
  display: block;
  font-size: 18px;
  margin-bottom: 4px;
  opacity: 0.8;
}

/* TABLE BODY */
.pasaran-table tbody tr {
  border-bottom: 1px solid rgba(255, 255, 255, 0.04);
  transition: all 0.3s ease;
  position: relative;
  animation: tableRowGlow 4s ease-in-out infinite;
}

.pasaran-table tbody tr:nth-child(even) {
  background: rgba(255, 255, 255, 0.015);
}

.pasaran-table tbody tr:hover {
  background: rgba(255, 215, 0, 0.06) !important;
  transform: scale(1.01);
  box-shadow:
    0 4px 20px rgba(0, 0, 0, 0.3),
    inset 0 0 0 1px rgba(255, 215, 0, 0.15);
}

.pasaran-table td {
  padding: 18px 24px;
  text-align: center;
  font-family: 'Rajdhani', sans-serif;
  font-size: 16px;
  font-weight: 600;
  color: rgba(44, 42, 42, 0.85);
  transition: all 0.3s ease;
  position: relative;
}

.pasaran-table tbody tr:hover td {
  color: #222121;
}

/* Kolom pertama (nama pasaran) */
.pasaran-table td:first-child {
  font-family: 'Orbitron', sans-serif;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 0.5px;
  color: #222121;
  text-align: left;
  padding-left: 28px;
}

/* Badge nama pasaran */
.pasaran-name {
  display: inline-flex;
  align-items: center;
  gap: 10px;
}

.pasaran-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  flex-shrink: 0;
  animation: glowPulse 2s ease-in-out infinite;
}

/* Warna dot berbeda tiap baris */
.pasaran-table tbody tr:nth-child(1) .pasaran-dot { background: #ffd700; box-shadow: 0 0 8px #ffd700; }
.pasaran-table tbody tr:nth-child(2) .pasaran-dot { background: #00e1ff; box-shadow: 0 0 8px #00e1ff; }
.pasaran-table tbody tr:nth-child(3) .pasaran-dot { background: #ff4d4d; box-shadow: 0 0 8px #ff4d4d; }
.pasaran-table tbody tr:nth-child(4) .pasaran-dot { background: #00ff88; box-shadow: 0 0 8px #00ff88; }
.pasaran-table tbody tr:nth-child(5) .pasaran-dot { background: #bf00ff; box-shadow: 0 0 8px #bf00ff; }

/* Badge frekuensi */
.freq-badge {
  display: inline-block;
  padding: 4px 14px;
  border-radius: 50px;
  font-family: 'Rajdhani', sans-serif;
  font-size: 13px;
  font-weight: 700;
  background: rgba(255, 215, 0, 0.1);
  border: 1px solid rgba(255, 215, 0, 0.2);
  color: #ff0000;
  letter-spacing: 0.5px;
  transition: all 0.3s ease;
}

.pasaran-table tbody tr:hover .freq-badge {
  background: rgba(255, 215, 0, 0.2);
  border-color: rgba(255, 215, 0, 0.5);
  box-shadow: 0 0 10px rgba(255, 215, 0, 0.2);
}

/* Waktu penutupan */
.time-wrap {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-family: 'Orbitron', sans-serif;
  font-size: 13px;
  font-weight: 700;
  color: #00e1ff;
  letter-spacing: 1px;
}

.time-icon {
  font-size: 14px;
  animation: countdownBlink 2s ease-in-out infinite;
}

/* Status LIVE */
.live-badge {
  display: inline-flex;
  align-items: center;
  gap: 5px;
  padding: 3px 10px;
  background: rgba(0, 255, 100, 0.1);
  border: 1px solid rgba(0, 255, 100, 0.3);
  border-radius: 50px;
  font-family: 'Orbitron', sans-serif;
  font-size: 9px;
  font-weight: 700;
  color: #00ff88;
  letter-spacing: 1px;
  margin-left: 8px;
}

.live-dot {
  width: 5px;
  height: 5px;
  border-radius: 50%;
  background: #00ff88;
  box-shadow: 0 0 6px #00ff88;
  animation: countdownBlink 1s ease-in-out infinite;
}

/* ============================================
   TABLE FOOTER INFO
============================================ */
.table-footer-info {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  margin-top: 30px;
  flex-wrap: wrap;
  animation: fadeInUp 0.8s ease-out 0.5s both;
}

.info-chip {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 10px 20px;
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 50px;
  font-family: 'Rajdhani', sans-serif;
  font-size: 13px;
  font-weight: 600;
  color: rgba(255, 255, 255, 0.6);
  letter-spacing: 0.5px;
  transition: all 0.3s ease;
  backdrop-filter: blur(10px);
}

.info-chip:hover {
  background: rgba(255, 215, 0, 0.08);
  border-color: rgba(255, 215, 0, 0.25);
  color: #ffd700;
  transform: translateY(-2px);
  box-shadow: 0 4px 15px rgba(255, 215, 0, 0.15);
}

.info-chip-icon {
  font-size: 16px;
}

/* ============================================
   STATS ROW
============================================ */
.stats-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-bottom: 50px;
  flex-wrap: wrap;
  animation: fadeInUp 0.8s ease-out 0.2s both;
}

.stat-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  padding: 16px 28px;
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 215, 0, 0.12);
  border-radius: 14px;
  backdrop-filter: blur(10px);
  transition: all 0.3s ease;
  min-width: 120px;
}

.stat-card:hover {
  background: rgba(255, 215, 0, 0.07);
  border-color: rgba(255, 0, 0, 0.2);
  transform: translateY(-4px);
  box-shadow: 0 8px 25px rgba(255, 215, 0, 0.15);
}

.stat-number {
  font-family: 'Orbitron', sans-serif;
  font-size: 26px;
  font-weight: 900;
  background: linear-gradient(135deg, #ffd700, #ff8c00);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  line-height: 1;
}

.stat-label {
  font-family: 'Rajdhani', sans-serif;
  font-size: 12px;
  font-weight: 600;
  color: rgba(255, 255, 255, 0.5);
  letter-spacing: 1px;
  text-transform: uppercase;
}

/* ============================================
   RESPONSIVE
============================================ */
@media (max-width: 768px) {

  .cara-daftar,
  .situs-judi {
    padding: 60px 16px 80px;
  }

  .cara-daftar h2,
  .situs-judi h2 {
    font-size: 24px;
    line-height: 1.3;
  }

  .section-badge {
    font-size: 9px;
    letter-spacing: 2px;
    padding: 5px 14px;
  }

  .cara-daftar-intro,
  .cara-daftar-outro {
    font-size: 14px;
  }

  .steps-container::before {
    left: 24px;
  }

  .step-item {
    padding: 16px 16px;
    gap: 14px;
  }

  .step-number {
    width: 42px;
    height: 42px;
    font-size: 15px;
  }

  .step-title {
    font-size: 15px;
  }

  .step-desc {
    font-size: 12px;
  }

  .step-icon {
    display: none;
  }

  .cta-daftar {
    padding: 14px 32px;
    font-size: 12px;
    letter-spacing: 1.5px;
  }

  .stats-row {
    gap: 12px;
  }

  .stat-card {
    padding: 12px 18px;
    min-width: 90px;
  }

  .stat-number {
    font-size: 20px;
  }

  .stat-label {
    font-size: 10px;
  }

  /* Table responsive */
  .table-border-glow {
    border-radius: 14px;
    padding: 1.5px;
  }

  .pasaran-table th {
    padding: 14px 12px;
    font-size: 10px;
    letter-spacing: 0.5px;
  }

  .th-icon {
    font-size: 14px;
  }

  .pasaran-table td {
    padding: 14px 10px;
    font-size: 13px;
  }

  .pasaran-table td:first-child {
    font-size: 10px;
    padding-left: 14px;
  }

  .freq-badge {
    font-size: 11px;
    padding: 3px 10px;
  }

  .time-wrap {
    font-size: 11px;
    gap: 4px;
  }

  .live-badge {
    display: none;
  }

  .table-footer-info {
    gap: 10px;
  }

  .info-chip {
    font-size: 11px;
    padding: 8px 14px;
  }
}

@media (max-width: 480px) {
  .cara-daftar h2,
  .situs-judi h2 {
    font-size: 20px;
  }

  .pasaran-table th:nth-child(2),
  .pasaran-table td:nth-child(2) {
    display: none;
  }

  .stat-card {
    min-width: 80px;
    padding: 10px 14px;
  }
}

</style>

<!-- ============================================
     HTML SECTION CARA DAFTAR
============================================ -->
<section class="cara-daftar">

  <!-- Partikel dekorasi -->
  <div class="particle-wrap">
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
  </div>

  <!-- Judul -->
  <div class="section-title-wrap">
    <div class="section-badge">✦ PANDUAN BERGABUNG ✦</div>
    <h2>Langkah Mudah Bergabung<br>di AI MR SULTAN</h2>
    <div class="title-underline">
      <span></span>
      <div class="title-underline-dot"></div>
      <span></span>
    </div>
  </div>

  <!-- Intro -->
  <p class="cara-daftar-intro">
    Untuk mulai menggunakan platform ini, berikut langkah-langkah
    yang umum dilakukan. Proses pendaftaran cepat, mudah, dan aman
    hanya dalam beberapa menit saja.
  </p>

  <!-- Stats Row -->
  <div class="stats-row">
    <div class="stat-card">
      <span class="stat-number">5</span>
      <span class="stat-label">Langkah</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">3<span style="font-size:16px">mnt</span></span>
      <span class="stat-label">Proses Daftar</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">24/7</span>
      <span class="stat-label">Layanan</span>
    </div>
    <div class="stat-card">
      <span class="stat-number">100%</span>
      <span class="stat-label">Aman</span>
    </div>
  </div>

  <!-- Steps -->
  <div class="steps-container">

    <div class="step-item">
      <div class="step-number">01</div>
      <div class="step-content">
        <div class="step-title">Kunjungi Link Login Resmi AI MR SULTAN</div>
        <div class="step-desc">
          Buka browser Anda dan akses situs resmi AI MR SULTAN melalui
          link yang telah tersedia. Pastikan Anda mengakses link yang benar
          dan terpercaya.
        </div>
      </div>
      <div class="step-icon">🌐</div>
    </div>

    <div class="step-item">
      <div class="step-number">02</div>
      <div class="step-content">
        <div class="step-title">Klik Tombol Daftar</div>
        <div class="step-desc">
          Temukan dan klik tombol <strong style="color:#ffd700">DAFTAR</strong>
          yang tersedia di halaman utama. Isi formulir pendaftaran dengan
          data diri yang valid dan lengkap.
        </div>
      </div>
      <div class="step-icon">📝</div>
    </div>

    <div class="step-item">
      <div class="step-number">03</div>
      <div class="step-content">
        <div class="step-title">Verifikasi Akun Anda</div>
        <div class="step-desc">
          Lakukan verifikasi akun melalui nomor telepon atau email
          yang telah Anda daftarkan. Proses verifikasi berlangsung
          cepat dan mudah.
        </div>
      </div>
      <div class="step-icon">✅</div>
    </div>

    <div class="step-item">
      <div class="step-number">04</div>
      <div class="step-content">
        <div class="step-title">Lakukan Deposit Awal</div>
        <div class="step-desc">
          Isi saldo akun Anda dengan melakukan deposit melalui berbagai
          metode pembayaran yang tersedia. Proses deposit cepat dan
          langsung masuk ke akun Anda.
        </div>
      </div>
      <div class="step-icon">💰</div>
    </div>

    <div class="step-item">
      <div class="step-number">05</div>
      <div class="step-content">
        <div class="step-title">Mulai Bermain & Raih Kemenangan</div>
        <div class="step-desc">
          Selamat! Akun Anda siap digunakan. Pilih pasaran favorit Anda,
          bermain dengan santai, dan raih kemenangan bersama AI MR SULTAN.
        </div>
      </div>
      <div class="step-icon">🏆</div>
    </div>

  </div>

  <!-- Outro -->
  <p class="cara-daftar-outro">
    Cara di atas ini praktis dan mudah bagi para pemula yang ingin bermain.
    Tim support kami siap membantu Anda 24 jam sehari, 7 hari seminggu.
  </p>

  <!-- CTA Button -->
  <div class="cta-wrap">
    <a href="https://vanillacafes.com/matcha-latte/"
       rel="nofollow noopener" target="_blank"
       class="cta-daftar">
      <span>DAFTAR SEKARANG</span>
      <span class="cta-arrow">→</span>
    </a>
  </div>

</section>

<!-- ============================================
     HTML SECTION BANDAR SLOT / PASARAN
============================================ -->
<section class="situs-judi">

  <!-- Partikel dekorasi -->
  <div class="particle-wrap">
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
  </div>

  <!-- Judul -->
  <div class="section-title-wrap">
    <div class="section-badge">✦ PASARAN TERSEDIA ✦</div>
    <h2>Pilihan Pasaran Togel<br>Terlengkap & Terpercaya</h2>
    <div class="title-underline">
      <span></span>
      <div class="title-underline-dot"></div>
      <span></span>
    </div>
  </div>

  <!-- Tabel Pasaran -->
  <div class="table-wrapper">
    <div class="table-border-glow">
      <table class="pasaran-table">

        <!-- HEADER -->
        <thead>
          <tr>
            <th>
              <span class="th-icon">🎯</span>
              NAMA PASARAN
            </th>
            <th>
              <span class="th-icon">🔄</span>
              FREKUENSI DRAW
            </th>
            <th>
              <span class="th-icon">⏰</span>
              WAKTU PENUTUPAN
            </th>
          </tr>
        </thead>

        <!-- BODY -->
        <tbody>
          <tr>
            <td>
              <div class="pasaran-name">
                <span class="pasaran-dot"></span>
                TOTO MACAU POOLS
                <span class="live-badge">
                  <span class="live-dot"></span>
                  LIVE
                </span>
              </div>
            </td>
            <td>
              <span class="freq-badge">Beberapa Kali Sehari</span>
            </td>
            <td>
              <div class="time-wrap">
                <span class="time-icon">⏱</span>
                Bervariasi per Sesi
              </div>
            </td>
          </tr>

          <tr>
            <td>
              <div class="pasaran-name">
                <span class="pasaran-dot"></span>
                MUNCHEN LOTTERIES
                <span class="live-badge">
                  <span class="live-dot"></span>
                  LIVE
                </span>
              </div>
            </td>
            <td>
              <span class="freq-badge">Harian</span>
            </td>
            <td>
              <div class="time-wrap">
                <span class="time-icon">⏱</span>
                22:45 WIB
              </div>
            </td>
          </tr>

          <tr>
            <td>
              <div class="pasaran-name">
                <span class="pasaran-dot"></span>
                HONGKONG LOTTO
                <span class="live-badge">
                <span class="live-dot"></span>
                LIVE
              </span>
            </div>
          </td>
          <td>
            <span class="freq-badge">Harian</span>
          </td>
          <td>
            <div class="time-wrap">
              <span class="time-icon">⏱</span>
              22:59 WIB
            </div>
          </td>
        </tr>

        <tr>
          <td>
            <div class="pasaran-name">
              <span class="pasaran-dot"></span>
              SYDNEY LOTTO
              <span class="live-badge">
                <span class="live-dot"></span>
                LIVE
              </span>
            </div>
          </td>
          <td>
            <span class="freq-badge">Harian</span>
          </td>
          <td>
            <div class="time-wrap">
              <span class="time-icon">⏱</span>
              13:49 WIB
            </div>
          </td>
        </tr>

        <tr>
          <td>
            <div class="pasaran-name">
              <span class="pasaran-dot"></span>
              BOSTON LOTTERIES
              <span class="live-badge">
                <span class="live-dot"></span>
                LIVE
              </span>
            </div>
          </td>
          <td>
            <span class="freq-badge">Harian</span>
          </td>
          <td>
            <div class="time-wrap">
              <span class="time-icon">⏱</span>
              23:50 WIB
            </div>
          </td>
        </tr>
      </tbody>

    </table>
  </div>
</div>

<!-- Info Chips -->
<div class="table-footer-info">
  <div class="info-chip">
    <span class="info-chip-icon">🔒</span>
    Sistem Keamanan Terjamin
  </div>
  <div class="info-chip">
    <span class="info-chip-icon">⚡</span>
    Result Real-Time
  </div>
  <div class="info-chip">
    <span class="info-chip-icon">💎</span>
    Odds Terbaik
  </div>
  <div class="info-chip">
    <span class="info-chip-icon">🎁</span>
    Bonus Menarik
  </div>
</div>

</section>

<!-- ============================================
   JAVASCRIPT INTERAKTIF
============================================ -->
<script>
(function () {

/* ============================================
   INTERSECTION OBSERVER - Animasi Masuk
============================================ */
var observerOptions = {
  threshold: 0.15,
  rootMargin: '0px 0px -50px 0px'
};

var observer = new IntersectionObserver(function (entries) {
  entries.forEach(function (entry) {
    if (entry.isIntersecting) {
      entry.target.classList.add('is-visible');
      observer.unobserve(entry.target);
    }
  });
}, observerOptions);

/* Observe semua step item */
document.querySelectorAll('.step-item').forEach(function (el, i) {
  el.style.opacity = '0';
  el.style.transform = 'translateX(-40px)';
  el.style.transition = 'opacity 0.6s ease ' + (i * 0.12) + 's, transform 0.6s ease ' + (i * 0.12) + 's';
  observer.observe(el);
});

/* Observe stat cards */
document.querySelectorAll('.stat-card').forEach(function (el, i) {
  el.style.opacity = '0';
  el.style.transform = 'translateY(30px)';
  el.style.transition = 'opacity 0.5s ease ' + (i * 0.1) + 's, transform 0.5s ease ' + (i * 0.1) + 's';
  observer.observe(el);
});

/* Observe table rows */
document.querySelectorAll('.pasaran-table tbody tr').forEach(function (el, i) {
  el.style.opacity = '0';
  el.style.transform = 'translateX(30px)';
  el.style.transition = 'opacity 0.5s ease ' + (i * 0.1) + 's, transform 0.5s ease ' + (i * 0.1) + 's';
  observer.observe(el);
});

/* Observe info chips */
document.querySelectorAll('.info-chip').forEach(function (el, i) {
  el.style.opacity = '0';
  el.style.transform = 'translateY(20px)';
  el.style.transition = 'opacity 0.4s ease ' + (i * 0.1) + 's, transform 0.4s ease ' + (i * 0.1) + 's';
  observer.observe(el);
});

/* Tambahkan class is-visible */
var styleVisible = document.createElement('style');
styleVisible.textContent = '.is-visible { opacity: 1 !important; transform: none !important; }';
document.head.appendChild(styleVisible);

/* ============================================
   COUNTER ANIMASI ANGKA STATS
============================================ */
function animateCounter(el, target, suffix, duration) {
  var start = 0;
  var startTime = null;
  var isDecimal = target % 1 !== 0;

  function step(timestamp) {
    if (!startTime) startTime = timestamp;
    var progress = Math.min((timestamp - startTime) / duration, 1);
    var eased = 1 - Math.pow(1 - progress, 3);
    var current = isDecimal
      ? (eased * target).toFixed(1)
      : Math.floor(eased * target);
    el.textContent = current + suffix;
    if (progress < 1) requestAnimationFrame(step);
  }
  requestAnimationFrame(step);
}

/* Observer khusus stats */
var statsObserver = new IntersectionObserver(function (entries) {
  entries.forEach(function (entry) {
    if (entry.isIntersecting) {
      var numbers = entry.target.querySelectorAll('.stat-number');
      numbers.forEach(function (numEl) {
        var text = numEl.textContent.trim();
        if (text === '5')    animateCounter(numEl, 5,    '',   1000);
        if (text.includes('mnt')) {
          numEl.innerHTML = '3<span style="font-size:16px">mnt</span>';
        }
        if (text === '100%') animateCounter(numEl, 100,  '%',  1500);
      });
      statsObserver.unobserve(entry.target);
    }
  });
}, { threshold: 0.5 });

var statsRow = document.querySelector('.stats-row');
if (statsRow) statsObserver.observe(statsRow);

/* ============================================
   HOVER RIPPLE PADA TABLE ROW
============================================ */
document.querySelectorAll('.pasaran-table tbody tr').forEach(function (row) {
  row.addEventListener('mouseenter', function () {
    this.style.transition = 'all 0.3s ease';
  });
});

/* ============================================
   STEP ITEM - KLIK EXPAND DETAIL
============================================ */
document.querySelectorAll('.step-item').forEach(function (item) {
  item.style.cursor = 'pointer';
  item.addEventListener('click', function () {
    var allItems = document.querySelectorAll('.step-item');
    allItems.forEach(function (i) {
      if (i !== item) {
        i.style.background = '';
        i.style.borderColor = '';
        i.querySelector('.step-number').style.background = '';
        i.querySelector('.step-number').style.color = '';
        i.querySelector('.step-number').style.borderColor = '';
      }
    });

    var isActive = item.dataset.active === 'true';
    if (!isActive) {
      item.style.background = 'rgba(255, 215, 0, 0.08)';
      item.style.borderColor = 'rgba(255, 0, 0, 0.25)';
      var num = item.querySelector('.step-number');
      num.style.background = 'linear-gradient(145deg, #ffd700, #ff8c00)';
      num.style.color = '#000';
      num.style.borderColor = '#ffd700';
      item.dataset.active = 'true';
    } else {
      item.style.background = '';
      item.style.borderColor = '';
      var num2 = item.querySelector('.step-number');
      num2.style.background = '';
      num2.style.color = '';
      num2.style.borderColor = '';
      item.dataset.active = 'false';
    }
  });
});

/* ============================================
   WAKTU REAL-TIME UPDATE
============================================ */
function updateTimes() {
  var now = new Date();
  var wibOffset = 7 * 60;
  var utc = now.getTime() + (now.getTimezoneOffset() * 60000);
  var wib = new Date(utc + (wibOffset * 60000));

  var h = String(wib.getHours()).padStart(2, '0');
  var m = String(wib.getMinutes()).padStart(2, '0');
  var s = String(wib.getSeconds()).padStart(2, '0');

  var clockEl = document.getElementById('live-clock');
  if (clockEl) clockEl.textContent = h + ':' + m + ':' + s + ' WIB';
}

setInterval(updateTimes, 1000);
updateTimes();

/* ============================================
   TABEL ROW - HIGHLIGHT PASARAN AKTIF
============================================ */
var pasaranSchedule = [
  { row: 0, closeHour: 23, closeMin: 59 }, /* Macau - bervariasi */
  { row: 1, closeHour: 17, closeMin: 45 }, /* SG7Days */
  { row: 2, closeHour: 22, closeMin: 59 }, /* HK */
  { row: 3, closeHour: 13, closeMin: 49 }, /* Sydney */
  { row: 4, closeHour: 23, closeMin: 45 }, /* Kowloon */
];

function highlightActiveMarket() {
  var now = new Date();
  var wibOffset = 7 * 60;
  var utc = now.getTime() + (now.getTimezoneOffset() * 60000);
  var wib = new Date(utc + (wibOffset * 60000));
  var currentMinutes = wib.getHours() * 60 + wib.getMinutes();

  var rows = document.querySelectorAll('.pasaran-table tbody tr');

  pasaranSchedule.forEach(function (schedule) {
    var row = rows[schedule.row];
    if (!row) return;

    var closeMinutes = schedule.closeHour * 60 + schedule.closeMin;
    var openMinutes  = closeMinutes - 240; /* buka 4 jam sebelum tutup */

    var isOpen = currentMinutes >= openMinutes && currentMinutes < closeMinutes;

    if (isOpen) {
      row.style.background = 'rgba(0, 255, 136, 0.04)';
      row.style.borderLeft  = '3px solid rgba(0, 255, 136, 0.5)';
    }
  });
}

highlightActiveMarket();
setInterval(highlightActiveMarket, 60000);

})();
</script>
<style>
/* ============================================
   IMPORT FONT
============================================ */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@400;600;700&display=swap');

/* ============================================
   KEYFRAME ANIMATIONS
============================================ */
@keyframes footerGlow {
  0%, 100% { box-shadow: 0 -4px 30px rgba(255, 200, 0, 0.4), 0 -1px 15px rgba(255, 150, 0, 0.3), inset 0 1px 0 rgba(255, 220, 50, 0.3); }
  50%       { box-shadow: 0 -4px 50px rgba(255, 200, 0, 0.8), 0 -1px 25px rgba(255, 150, 0, 0.6), inset 0 1px 0 rgba(255, 220, 50, 0.6); }
}

@keyframes borderShimmer {
  0%   { background-position: 0% 50%; }
  50%  { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

@keyframes iconFloat {
  0%, 100% { transform: translateY(0px); }
  50%       { transform: translateY(-3px); }
}

@keyframes iconPulse {
  0%, 100% { filter: drop-shadow(0 0 4px rgba(255, 200, 0, 0.6)); }
  50%       { filter: drop-shadow(0 0 10px rgba(255, 200, 0, 1)); }
}

@keyframes centerPulse {
  0%, 100% {
    transform: translateY(-22px) scale(1);
    box-shadow:
      0 0 0 0 rgba(255, 200, 0, 0.7),
      0 8px 25px rgba(255, 150, 0, 0.5),
      inset 0 1px 0 rgba(255, 255, 255, 0.3);
  }
  50% {
    transform: translateY(-22px) scale(1.05);
    box-shadow:
      0 0 0 12px rgba(255, 200, 0, 0),
      0 8px 35px rgba(255, 150, 0, 0.8),
      inset 0 1px 0 rgba(255, 255, 255, 0.4);
  }
}

@keyframes centerRing {
  0%   { transform: scale(1); opacity: 0.8; }
  100% { transform: scale(1.8); opacity: 0; }
}

@keyframes activeIndicator {
  0%, 100% { opacity: 1; transform: scaleX(1); }
  50%       { opacity: 0.6; transform: scaleX(0.7); }
}

@keyframes particleFloat {
  0%   { transform: translateY(0) translateX(0) scale(1); opacity: 1; }
  100% { transform: translateY(-40px) translateX(10px) scale(0); opacity: 0; }
}

@keyframes scanLine {
  0%   { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}

@keyframes textGlow {
  0%, 100% { text-shadow: 0 0 4px rgba(255, 200, 0, 0.5); }
  50%       { text-shadow: 0 0 10px rgba(255, 200, 0, 1), 0 0 20px rgba(255, 150, 0, 0.5); }
}

@keyframes ripple {
  0%   { transform: scale(0); opacity: 1; }
  100% { transform: scale(4); opacity: 0; }
}

@keyframes slideUp {
  from { transform: translateY(100px); opacity: 0; }
  to   { transform: translateY(0); opacity: 1; }
}

/* ============================================
   FOOTER WRAPPER
============================================ */
.RKBM-fixed-footer {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 9999;
  display: flex;
  justify-content: space-around;
  align-items: flex-end;
  padding: 0 8px 6px;
  height: 72px;

  /* Background utama */
  background: linear-gradient(
    180deg,
    #1a1a2e 0%,
    #0d0d1a 40%,
    #000000 100%
  );

  /* Border radius atas */
  border-radius: 28px 28px 0 0;

  /* Animasi glow */
  animation: footerGlow 3s ease-in-out infinite, slideUp 0.5s ease-out;

  /* Overflow untuk efek dalam */
  overflow: visible;
}

/* Garis border atas animasi */
.RKBM-fixed-footer::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    #ff6b00 15%,
    #ffd700 30%,
    #ffffff 50%,
    #ffd700 70%,
    #ff6b00 85%,
    transparent 100%
  );
  background-size: 200% 100%;
  animation: borderShimmer 3s linear infinite;
  border-radius: 28px 28px 0 0;
}

/* Scan line effect */
.RKBM-fixed-footer::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(
    90deg,
    transparent 0%,
    rgba(255, 0, 0, 0.025) 50%,
    transparent 100%
  );
  width: 60%;
  animation: scanLine 4s linear infinite;
  pointer-events: none;
  border-radius: 28px 28px 0 0;
}

/* ============================================
   FOOTER ITEM (LINK)
============================================ */
.RKBM-fixed-footer a {
  position: relative;
  flex: 1;
  text-decoration: none;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
  padding-bottom: 4px;
  gap: 3px;
  color: rgba(255, 255, 255, 0.6);
  font-size: 9px;
  font-family: 'Rajdhani', 'Orbitron', sans-serif;
  font-weight: 600;
  letter-spacing: 0.5px;
  text-transform: uppercase;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
  cursor: pointer;
  -webkit-tap-highlight-color: transparent;
  max-width: 80px;
  height: 100%;
  overflow: visible;
}

/* Ripple effect on click */
.RKBM-fixed-footer a .ripple-effect {
  position: absolute;
  border-radius: 50%;
  background: rgba(255, 200, 0, 0.3);
  animation: ripple 0.6s linear;
  pointer-events: none;
  width: 20px;
  height: 20px;
}

/* ============================================
   ICON WRAPPER
============================================ */
.footer-icon-wrap {
  position: relative;
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 12px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.08);
  transition: all 0.3s ease;
  margin-bottom: 1px;
}

.RKBM-fixed-footer a:hover .footer-icon-wrap,
.RKBM-fixed-footer a.active .footer-icon-wrap {
  background: rgba(255, 200, 0, 0.15);
  border-color: rgba(255, 200, 0, 0.4);
  box-shadow: 0 0 15px rgba(255, 200, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.1);
}

/* ============================================
   ICON IMAGE
============================================ */
.RKBM-fixed-footer img {
  width: 22px;
  height: 22px;
  object-fit: contain;
  transition: all 0.3s ease;
  filter: brightness(0.7) saturate(0.5);
  position: relative;
  z-index: 2;
}

.RKBM-fixed-footer a:hover img,
.RKBM-fixed-footer a.active img {
  filter: brightness(1.2) saturate(1.5) drop-shadow(0 0 6px rgba(255, 200, 0, 0.8));
  animation: iconFloat 2s ease-in-out infinite, iconPulse 2s ease-in-out infinite;
}

/* ============================================
   LABEL TEXT
============================================ */
.footer-label {
  font-size: 8.5px;
  font-family: 'Rajdhani', sans-serif;
  font-weight: 700;
  letter-spacing: 0.8px;
  color: rgba(255, 255, 255, 0.5);
  transition: all 0.3s ease;
  white-space: nowrap;
}

.RKBM-fixed-footer a:hover .footer-label,
.RKBM-fixed-footer a.active .footer-label {
  color: #ffd700;
  animation: textGlow 2s ease-in-out infinite;
}

/* ============================================
   ACTIVE INDICATOR DOT
============================================ */
.footer-dot {
  width: 4px;
  height: 4px;
  border-radius: 50%;
  background: #ffd700;
  position: absolute;
  bottom: 2px;
  left: 50%;
  transform: translateX(-50%) scale(0);
  transition: transform 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
  box-shadow: 0 0 6px #ffd700;
}

.RKBM-fixed-footer a:hover .footer-dot,
.RKBM-fixed-footer a.active .footer-dot {
  transform: translateX(-50%) scale(1);
  position: relative;
  z-index: 10000;
  animation: activeIndicator 1.5s ease-in-out infinite;
}

/* ============================================
   CENTER BUTTON (DAFTAR) - SPECIAL
============================================ */
.RKBM-fixed-footer a.center-btn {
  position: relative;
  justify-content: flex-start;
  padding-top: 0;
  margin-top: -28px;
}

.center-btn-inner {
  position: relative;
  z-index: 9999;
  width: 158px;
  height: 308px;
  border-radius: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2px;

  /* Gradient emas premium */
  background: linear-gradient(
    145deg,
    #ff8c00 0%,
    #ffd700 30%,
    #ffec6e 50%,
    #ffd700 70%,
    #ff8c00 100%
  );

  /* Shadow megah */
  box-shadow:
    0 0 0 3px rgba(255, 0, 0, 0.2),
    0 0 0 6px rgba(200, 0, 0, 0.15),
    0 8px 25px rgba(255, 150, 0, 0.6),
    0 4px 10px rgba(0, 0, 0, 0.5),
    inset 0 2px 4px rgba(255, 255, 255, 0.4),
    inset 0 -2px 4px rgba(0, 0, 0, 0.2);

  animation: centerPulse 2.5s ease-in-out infinite;
  transition: all 0.3s ease;
  cursor: pointer;
}

/* Ring animasi di sekitar tombol center */
.center-btn-inner::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  border: 2px solid rgba(255, 215, 0, 0.6);
  animation: centerRing 2s ease-out infinite;
}

.center-btn-inner::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  border: 2px solid rgba(255, 150, 0, 0.4);
  animation: centerRing 2s ease-out infinite 0.5s;
}

.center-btn-inner img {
  width: 26px;
  height: 26px;
  filter: brightness(0) invert(1) drop-shadow(0 1px 2px rgba(0,0,0,0.5)) !important;
  animation: none !important;
}

.RKBM-fixed-footer a.center-btn:hover .center-btn-inner {
  transform: translateY(-5px) scale(1.08);
  box-shadow:
    0 0 0 4px rgba(255, 215, 0, 0.5),
    0 0 0 8px rgba(255, 150, 0, 0.2),
    0 15px 35px rgba(255, 150, 0, 0.8),
    0 6px 15px rgba(0, 0, 0, 0.5),
    inset 0 2px 4px rgba(255, 255, 255, 0.5);
}

.center-btn-label {
  font-size: 8px;
  font-family: 'Orbitron', sans-serif;
  font-weight: 900;
  color: #1a0a00;
  letter-spacing: 0.5px;
  text-shadow: 0 1px 0 rgba(255, 255, 255, 0.3);
  line-height: 1;
}

/* Label bawah tombol center */
.center-btn-text {
  font-size: 8.5px;
  font-family: 'Rajdhani', sans-serif;
  font-weight: 700;
  color: #ffd700;
  letter-spacing: 1px;
  text-shadow: 0 0 8px rgba(255, 200, 0, 0.8);
  margin-top: 4px;
  animation: textGlow 2s ease-in-out infinite;
}

/* ============================================
   BADGE NOTIFIKASI
============================================ */
.footer-badge {
  position: absolute;
  top: -4px;
  right: -4px;
  width: 16px;
  height: 16px;
  border-radius: 50%;
  background: linear-gradient(135deg, #ff0000, #ff6b6b);
  color: #fff;
  font-size: 8px;
  font-weight: 900;
  font-family: 'Orbitron', sans-serif;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 1.5px solid #1a1a2e;
  box-shadow: 0 0 8px rgba(255, 0, 0, 0.6);
  z-index: 10;
  animation: centerRing 1.5s ease-out infinite;
}

/* ============================================
   DIVIDER VERTIKAL ANTAR ITEM
============================================ */
.footer-divider {
  width: 1px;
  height: 30px;
  background: linear-gradient(
    180deg,
    transparent 0%,
    rgba(255, 215, 0, 0.2) 50%,
    transparent 100%
  );
  align-self: center;
  flex-shrink: 0;
}

/* ============================================
   HOVER BACKGROUND GLOW
============================================ */
.RKBM-fixed-footer a::before {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 100%;
  background: radial-gradient(
    ellipse at center top,
    rgba(255, 200, 0, 0.08) 0%,
    transparent 70%
  );
  transition: width 0.3s ease;
  border-radius: 0 0 20px 20px;
  pointer-events: none;
}

.RKBM-fixed-footer a:hover::before {
  width: 100%;
}

/* ============================================
   PARTICLES (dekorasi kecil)
============================================ */
.footer-particle {
  position: absolute;
  width: 3px;
  height: 3px;
  border-radius: 50%;
  background: #ffd700;
  pointer-events: none;
  opacity: 0;
}

.RKBM-fixed-footer a:hover .footer-particle:nth-child(1) {
  animation: particleFloat 1s ease-out 0s infinite;
  left: 30%;
  top: 20%;
}
.RKBM-fixed-footer a:hover .footer-particle:nth-child(2) {
  animation: particleFloat 1s ease-out 0.2s infinite;
  left: 60%;
  top: 30%;
}
.RKBM-fixed-footer a:hover .footer-particle:nth-child(3) {
  animation: particleFloat 1s ease-out 0.4s infinite;
  left: 45%;
  top: 15%;
}

/* ============================================
   RESPONSIVE MOBILE
============================================ */
@media (max-width: 360px) {
  .RKBM-fixed-footer {
    height: 65px;
    padding: 0 4px 4px;
  }
  .footer-icon-wrap {
    width: 30px;
    height: 30px;
    border-radius: 10px;
  }
  .RKBM-fixed-footer img {
    width: 18px;
    height: 18px;
  }
  .footer-label {
    font-size: 7.5px;
  }
  .center-btn-inner {
    width: 50px;
    height: 50px;
  }
  .center-btn-inner img {
    width: 22px !important;
    height: 22px !important;
  }
  .RKBM-fixed-footer a.center-btn {
    margin-top: -22px;
  }
}

@media (max-width: 320px) {
  .footer-label,
  .center-btn-text {
    font-size: 7px;
    letter-spacing: 0.3px;
  }
  .center-btn-inner {
    width: 46px;
    height: 46px;
  }
}

/* ============================================
   SAFE AREA (iPhone X+)
============================================ */
@supports (padding-bottom: env(safe-area-inset-bottom)) {
  .RKBM-fixed-footer {
    padding-bottom: calc(6px + env(safe-area-inset-bottom));
    height: calc(72px + env(safe-area-inset-bottom));
  }
}

/* ============================================
   BODY PADDING BAWAH
============================================ */
body {
  padding-bottom: 80px;
}

</style>

<!-- ============================================
     HTML FOOTER NAVIGASI
============================================ -->
<div class="RKBM-fixed-footer" id="mainFooter">

  <!-- PROMO -->
  <a href="https://vanillacafes.com/matcha-latte/"
     rel="nofollow noopener" target="_blank" id="btn-promo">
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <div class="footer-icon-wrap">
      <img src="https://italianspacefood.org/img/logo-firehorse-nikeslot88.webp"
           alt="Promo Ai Mr Sultan" width="22" height="22">
      <span class="footer-badge">5</span>
    </div>
    <span class="footer-label">PROMO</span>
    <span class="footer-dot"></span>
  </a>

  <div class="footer-divider"></div>

  <!-- LOGIN -->
  <a href="https://vanillacafes.com/matcha-latte/"
     rel="nofollow noopener" target="_blank" id="btn-login">
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <div class="footer-icon-wrap">
      <img src="https://italianspacefood.org/img/logo-firehorse-nikeslot88.webp"
           alt="Login Ai Mr Sultan" width="22" height="22">
    </div>
    <span class="footer-label">LOGIN</span>
    <span class="footer-dot"></span>
  </a>

  <div class="footer-divider"></div>

  <!-- DAFTAR (CENTER BUTTON) -->
  <a href="https://vanillacafes.com/matcha-latte/"
     rel="nofollow noopener" target="_blank"
     class="center-btn" id="btn-daftar">
    <div class="center-btn-inner">
      <img src="https://italianspacefood.org/img/logo-firehorse-nikeslot88.webp"
           alt="Daftar Ai Mr Sultan" width="26" height="26">
      <span class="center-btn-label">DAFTAR</span>
    </div>
    <span class="center-btn-text">DAFTAR</span>
  </a>

  <div class="footer-divider"></div>

  <!-- WHATSAPP -->
  <a href="https://vanillacafes.com/matcha-latte/"
     rel="nofollow noopener" target="_blank" id="btn-wa">
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <div class="footer-icon-wrap">
      <img src="https://italianspacefood.org/img/logo-firehorse-nikeslot88.webp"
           alt="WhatsApp Ai Mr Sultan" width="22" height="22">
    </div>
    <span class="footer-label">WHATSAPP</span>
    <span class="footer-dot"></span>
  </a>

  <div class="footer-divider"></div>

  <!-- LIVE CHAT -->
  <a href="https://vanillacafes.com/matcha-latte/"
     rel="nofollow noopener" target="_blank"
     class="js_live_chat_link live-chat-link" id="btn-livechat">
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <span class="footer-particle"></span>
    <div class="footer-icon-wrap">
      <img class="live-chat-icon"
           src="https://italianspacefood.org/img/logo-firehorse-nikeslot88.webp"
           alt="Live Chat Ai Mr Sultan" width="22" height="22">
      <!-- Indikator online -->
      <span style="
        position:absolute;
        bottom:4px; right:4px;
        width:7px; height:7px;
        border-radius:50%;
        background:#00ff88;
        border:1.5px solid #1a1a2e;
        box-shadow:0 0 6px #00ff88;
        animation:activeIndicator 1.5s ease-in-out infinite;
      "></span>
    </div>
    <span class="footer-label">LIVE CHAT</span>
    <span class="footer-dot"></span>
  </a>

</div>

<!-- ============================================
     JAVASCRIPT INTERAKTIF
============================================ -->
<script>
(function() {

  /* ---- Ripple Effect on Click ---- */
  document.querySelectorAll('.RKBM-fixed-footer a').forEach(function(btn) {
    btn.addEventListener('click', function(e) {
      var ripple = document.createElement('span');
      ripple.classList.add('ripple-effect');
      var rect = btn.getBoundingClientRect();
      var size = Math.max(rect.width, rect.height);
      ripple.style.width  = size + 'px';
      ripple.style.height = size + 'px';
      ripple.style.left   = (e.clientX - rect.left - size / 2) + 'px';
      ripple.style.top    = (e.clientY - rect.top  - size / 2) + 'px';
      btn.appendChild(ripple);
      setTimeout(function() { ripple.remove(); }, 700);
    });
  });

  /* ---- Active State ---- */
  document.querySelectorAll('.RKBM-fixed-footer a').forEach(function(btn) {
    btn.addEventListener('touchstart', function() {
      this.classList.add('active');
    }, { passive: true });
    btn.addEventListener('touchend', function() {
      var self = this;
      setTimeout(function() { self.classList.remove('active'); }, 300);
    }, { passive: true });
  });

  /* ---- Slide Up Animation on Load ---- */
  var footer = document.getElementById('mainFooter');
  if (footer) {
    footer.style.transform = 'translateY(100%)';
    footer.style.opacity   = '0';
    footer.style.transition = 'transform 0.6s cubic-bezier(0.34,1.56,0.64,1), opacity 0.4s ease';
    setTimeout(function() {
      footer.style.transform = 'translateY(0)';
      footer.style.opacity   = '1';
    }, 300);
  }

})();
</script>

<input type="hidden" id="page_title"
       value="Ai Mr Sultan - Bandar Situs Judi Slot Online Gacor & Link Slot88 Jackpot Terbesar" />

<script type="application/json" id="adobeAnalyticsProductData">
{
  "product_name": "Ai Mr Sultan - Bandar Situs Judi Slot Online Gacor & Link Slot88 Jackpot Terbesar",
  "mpn_id": "D-353465486A",
  "currency": "SGD",
  "product_price": {
    "sellingPrice": 259.0,
    "basePrice": 259.0
  },
  "brand": "AI MR SULTAN",
  "lob": "SLOT ONLINE",
  "sub_lob": "Ai Mr Sultan - Bandar Situs Judi Slot Online Gacor & Link Slot88 Jackpot Terbesar"
}
</script>
            <style>.slider_media video {max-width: 100%;}</style>
            
            <script>
               $(document).ready(function() {
                 $(document).on('click', '#apple-care-add', function (event) {
                   var isChecked = $('#add-apple-care').is(':checked');
                   if (isChecked) {
                     $('#add-apple-care').prop('checked', false);
                     $("#apple-care-add .pdp-care-btn").html("Add");
                     // $("#apple-added-if").val("");
                   } else {
                     $('#add-apple-care').prop('checked', true);
                     $("#apple-care-add .pdp-care-btn").html("Added");
                     // $("#apple-added-if").val("added");
                   }
                   var appleCareID = $(this).attr("data-index");
                   $("#apple-care-varid").val(appleCareID);
                   updatePriceAfterAddingCareOrWarranty();
                 });
                 $(document).on('click', '#secWarranty-add', function (event) {
                   var isChecked2 = $('#add-secWarranty').is(':checked');
                   if (isChecked2) {
                     $('#add-secWarranty').prop('checked', false);
                     $("#secWarranty-add .pdp-secWarranty-btn").html("Add");
                   } else {
                     $('#add-secWarranty').prop('checked', true);
                     $("#secWarranty-add .pdp-secWarranty-btn").html("Added");
                     // $("#apple-added-if").val("added");
                   }
                   var secWarrantyID = $(this).attr("data-index");
                   $("#secWarranty-varid").val(secWarrantyID);
                   updatePriceAfterAddingCareOrWarranty();
                 });
               
                 // Reset trade-in values to 0
                 $(document).on('click', '#no-trade-in', () => {
                   const $tradeInValueAmounts = document.querySelectorAll('.js-trade-in-value-amount');
                   const $startTradeInBtn = document.querySelector('.js-product-option-form .js-trade-in-modal-trigger-input');
                   const $startTradeInBtnLabel = document.querySelector('.js-product-option-form .js-trade-in-modal-trigger-input + label');
                   const $hiddenSelectedTradeIn = document.querySelector('#selected-trade-in-value');
                   const $productPrices = document.querySelectorAll('.js-product-price-with-care-warranty');
               
                   $tradeInValueAmounts.forEach(($tradeInValueAmount) => {
                     if ($tradeInValueAmount.classList?.contains('pdp-value-amount')) {
                       $tradeInValueAmount.innerText = '$0';
                       $tradeInValueAmount.setAttribute('data-trade-in-value', 0);
                       $tradeInValueAmount.parentElement?.classList?.add('hidden');
                     }
                   });
               
                   $startTradeInBtnLabel.innerText = 'Start trade-in';
                   $hiddenSelectedTradeIn.value = 0;
               
                   updatePriceAfterRemovingTradeIn();
                 });
               
                 function updatePriceAfterRemovingTradeIn() {
                   const isAppleCareAdded = $('#add-apple-care').is(':checked');
                   const isWarrantyAdded = $('#add-secWarranty').is(':checked');
                   const isTradeInAdded = document.querySelector('#selected-trade-in-value')?.value;
                   const $productPrices = document.querySelectorAll('.js-product-price-with-care-warranty');
               
                   $('.js-product-price-with-care-warranty').each((i, $productPrice) => {
                     const price = $($productPrice).data('price');
                     let updatedPrice;
               
                     /* TO BE ADDED */
                     if (isTradeInAdded && isAppleCareAdded && isWarrantyAdded) {
                       updatedPrice = $($productPrice).attr('data-price-with-care-and-secWarranty');
                     } else if (isTradeInAdded && isAppleCareAdded) {
                       updatedPrice = $($productPrice).attr('data-price-with-care');
                     } else if (isTradeInAdded && isWarrantyAdded) {
                       updatedPrice = $($productPrice).attr('data-price-with-secWarranty');
                     } else if (isTradeInAdded) {
                       updatedPrice = price;
                     } else {
                       updatedPrice = price;
                     }
               
                     $($productPrice).html(updatedPrice);
                   });
                 }
               
                 function updatePriceAfterAddingCareOrWarranty() {
                   const isAppleCareAdded = $('#add-apple-care').is(':checked');
                   const isWarrantyAdded = $('#add-secWarranty').is(':checked');
                   const hasTradeIn = $('#selected-trade-in-value').val() && $('#selected-trade-in-value').val() !== '0' && $("#selected-trade-in-device").val() !== '';
                   const hiddenSelectedTradeInValue = $('#selected-trade-in-value').val();
                   const tradeInPrice = hiddenSelectedTradeInValue
                     ? formatMoney(hiddenSelectedTradeInValue)
                     : 0;
               
                   $('.js-product-price-with-care-warranty').each(function(i, $productPrice) {
                     let price = $(this).attr('data-price');
                     const nmpPriceCalculation = $(this).data('priceCalculation');
               
                     if (isAppleCareAdded && isWarrantyAdded && hasTradeIn) {
                       price = setPriceWithTradeIn('data-price-with-care-and-secWarranty', $productPrice);
                     } else if (isAppleCareAdded && isWarrantyAdded) {
                       price = $(this).attr('data-price-with-care-and-secWarranty');
                     } else if (isAppleCareAdded && hasTradeIn) {
                       price = setPriceWithTradeIn('data-price-with-care', $productPrice);
                     } else if (isWarrantyAdded && hasTradeIn) {
                       price = setPriceWithTradeIn('data-price-with-secWarranty', $productPrice);
                     } else if (isAppleCareAdded) {
                       price = $(this).attr('data-price-with-care');
                     } else if (isWarrantyAdded) {
                       price = $(this).attr('data-price-with-secWarranty');
                     } else if (hasTradeIn) {
                       price = setPriceWithTradeIn('data-price', $productPrice);
                     }
               
                     $(this).html(price);
                   });
                 }
               
                 function setCookie(name, value, days) {
                   var expires = "";
                   if (days) {
                     var date = new Date();
                     date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
                     expires = "; expires=" + date.toUTCString();
                   }
                   document.cookie = name + "=" + (value || "") + expires + "; path=/";
                 }
               
                 function getCookie(name) {
                   var nameEQ = name + "=";
                   var ca = document.cookie.split(';');
                   for (var i = 0; i < ca.length; i++) {
                     var c = ca[i];
                     while (c.charAt(0) == ' ') c = c.substring(1, c.length);
                     if (c.indexOf(nameEQ) == 0) return c.substring(nameEQ.length, c.length);
                   }
                   return null;
                 }
               
                 function eraseCookie(name) {
                   document.cookie = name + '=; Path=/; Expires=Thu, 01 Jan 1970 00:00:01 GMT;';
                 }
               
                 //added by anusha - 4th variant option cookie approach - start
               
                 //check if the main product is inside 4th option product list. if its present, set cookie array
                 var pid = "7986665160884";
                 var pid1 = "";
                 var pid1 = pid1.replace(/s/g, "");
                 var pid2 = pid1.split('-');
                 var count = 0;
                 for (var j = 0; j < pid2.length; j++) {
                   var a = pid2[j];
                   var b = pid;
                   if (a.trim() == b.trim()) {
                     count++;
                   }
                 }
                 if (count > 0) {
                   setCookie('optionPIDlist', pid2.join('|'), {
                     path: '/'
                   });
                 }
               
                 // if the main product has 'empty 4th product list', then delete all the cookies
                 if (!pid1.length > 0) {
                   eraseCookie('option1select');
                   eraseCookie('option2select');
                   eraseCookie('option3select');
                   eraseCookie('optionPIDlist');
                 }
               
                 // cookie values - 3 options
                 let op1 = getCookie('option1select');
                 let op2 = getCookie('option2select');
                 let op3 = getCookie('option3select');
               
                 // when customer change the 4th option selection - trigger click event (inorder to set cookie values for 3 options)
                 if (op1 && $('fieldset.product-form__input[data-opcount="1"]').length > 0) {
                   setTimeout(function() {
                     $('fieldset.product-form__input[data-opcount="1"]').find('label[data-title="' + op1 + '"]').trigger('click');
                   }, 1000);
                 };
                 if (op2 && $('fieldset.product-form__input[data-opcount="2"]').length > 0) {
                   setTimeout(function() {
                     $('fieldset.product-form__input[data-opcount="2"]').find('label[data-title="' + op2 + '"]').trigger('click');
                   }, 1000);
                 };
                 if (op3 && $('fieldset.product-form__input[data-opcount="3"]').length > 0) {
                   setTimeout(function() {
                     $('fieldset.product-form__input[data-opcount="3"]').find('label[data-title="' + op3 + '"]').trigger('click');
                   }, 1000);
                 };
               
                 let op11 = $("input[type='radio'][name='Title']:checked").val();
                 let op22 = $("input[type='radio'][name='']:checked").val();
                 let op33 = $("input[type='radio'][name='']:checked").val();
               
                 // when customer dont click on any of the variant buttons - set cookie values for 3 options from current mainprod variant selection
                 if (op1 == null && op2 == null && op3 == null) {
                   if (op11 && $('fieldset.product-form__input[data-opcount="1"]').length > 0) {
                     setTimeout(function() {
                       $('fieldset.product-form__input[data-opcount="1"]').find('label[data-title="' + op11 + '"]').trigger('click');
                     }, 1000);
                   };
                   if (op22 && $('fieldset.product-form__input[data-opcount="2"]').length > 0) {
                     setTimeout(function() {
                       $('fieldset.product-form__input[data-opcount="2"]').find('label[data-title="' + op22 + '"]').trigger('click');
                     }, 1000);
                   };
                   if (op33 && $('fieldset.product-form__input[data-opcount="3"]').length > 0) {
                     setTimeout(function() {
                       $('fieldset.product-form__input[data-opcount="3"]').find('label[data-title="' + op33 + '"]').trigger('click');
                     }, 1000);
                   };
                   if (getCookie('optionPIDlist')) {
                     setCookie('option1select', op11, 7);
                     setCookie('option2select', op22, 7);
                     setCookie('option3select', op33, 7);
                   }
                 }
                 // added by anusha - 4th variant option cookie approach - end
               
                 if (vat_free_day == true) {
                   var vat_price_footer = $(".pricestyle").find(".vat_price_bold").text();
                   if (vat_price_footer != "") {
                     $("#price-element").find(".footerOr2").css("display", "none");
                   }
                 }
               });
            </script>
            <script>
               $(document).on('change', 'input[type="number"]', function (event) {
                 this.value = this.value.replace(/[^0-9]+/g, '');
                 if (this.value < 1) this.value = 0;
               });
               $(document).on('keypress', 'input[type="number"]', function (event) {
                 if (
                   (event.target.value.length == 0 && event.which == 48) ||
                   (event.target.value.length == 0 && event.which > 31 && event.which < 48) ||
                   (event.target.value.length == 0 && event.which > 57 && event.which < 128)
                 ) {
                   return false;
                 }
               });
               $(document).on('keypress', 'input[type="number"]', function (event) {
                 return (((event.which > 47) && (event.which < 58)) || (event.which == 13));
               });
               
               // reload page on back button click since the cached version on Safari browsers is incorrect
               $(window).bind("pageshow", function(event) {
                 if (event.originalEvent.persisted) {
                   window.location.reload();
                 }
               });
            </script>
            <style data-shopify>
               .add-on-product-style.add-on-product-style-secWarranty .care-pdp-title {
               /*     margin-left: 0; */
               }
            </style>
            <style> #shopify-section-template--17605519376564__main .accordion__content p a {color: var(--color-link-dynamic-label) !important;} #shopify-section-template--17605519376564__main .popup_round_border {display: none;} </style>
         </section>
         <div id="shopify-section-template--17605519376564__productMarketingContent" class="shopify-section">
            <link href="//www.istudiosg.com/cdn/shop/t/14/assets/productMarketingContent.css?v=134348870364535945721742784887" rel="stylesheet" type="text/css" media="all" />
            <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@400;600;700&family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
            <!-- haaaa....ngapain lagi hayo -->
            <style>
            
            /* ============================================
               KEYFRAMES
            ============================================ */
            @keyframes gradientShift {
              0%,100% { background-position: 0% 50%; }
              50%      { background-position: 100% 50%; }
            }
            @keyframes shimmerText {
              0%   { background-position: -200% center; }
              100% { background-position:  200% center; }
            }
            @keyframes glowPulse {
              0%,100% { box-shadow: 0 0 20px rgba(0,200,255,0.3), 0 0 40px rgba(0,150,255,0.1); }
              50%      { box-shadow: 0 0 40px rgba(0,200,255,0.7), 0 0 80px rgba(0,150,255,0.3); }
            }
            @keyframes borderRotate {
              0%   { background-position: 0% 50%; }
              100% { background-position: 400% 50%; }
            }
            @keyframes fadeInUp {
              from { opacity:0; transform:translateY(40px); }
              to   { opacity:1; transform:translateY(0); }
            }
            @keyframes fadeInLeft {
              from { opacity:0; transform:translateX(-30px); }
              to   { opacity:1; transform:translateX(0); }
            }
            @keyframes fadeInRight {
              from { opacity:0; transform:translateX(30px); }
              to   { opacity:1; transform:translateX(0); }
            }
            @keyframes floatUp {
              0%,100% { transform:translateY(0); }
              50%      { transform:translateY(-8px); }
            }
            @keyframes particleDrift {
              0%   { transform:translateY(0) translateX(0) rotate(0deg); opacity:1; }
              100% { transform:translateY(-120px) translateX(40px) rotate(360deg); opacity:0; }
            }
            @keyframes scanLine {
              0%   { background-position:0% 50%; }
              100% { background-position:400% 50%; }
            }
            @keyframes starPop {
              0%   { transform:scale(0) rotate(-30deg); opacity:0; }
              60%  { transform:scale(1.3) rotate(5deg); opacity:1; }
              100% { transform:scale(1) rotate(0deg); opacity:1; }
            }
            @keyframes cardEntrance {
              from { opacity:0; transform:translateY(50px) scale(0.95); }
              to   { opacity:1; transform:translateY(0) scale(1); }
            }
            @keyframes titleGlow {
              0%,100% { text-shadow: 0 0 10px rgba(0,200,255,0.5), 0 0 20px rgba(0,150,255,0.3); }
              50%      { text-shadow: 0 0 25px rgba(0,200,255,1), 0 0 50px rgba(0,150,255,0.6), 0 0 80px rgba(0,100,255,0.3); }
            }
            @keyframes lineExpand {
              from { width:0; }
              to   { width:80px; }
            }
            @keyframes countBlink {
              0%,100% { opacity:1; }
              50%      { opacity:0.4; }
            }
            @keyframes rotateRing {
              from { transform:rotate(0deg); }
              to   { transform:rotate(360deg); }
            }
            @keyframes progressBar {
              from { width:0%; }
              to   { width:var(--progress); }
            }
            
            /* ============================================
               WRAPPER UTAMA
            ============================================ */
            .RKBM-wrapper {
              position: relative;
              background:
                radial-gradient(ellipse at 15% 30%, rgba(255, 0, 0, 0.12) 0%, transparent 55%),
                radial-gradient(ellipse at 85% 70%, rgba(200, 0, 0, 0.1) 0%, transparent 55%),
                radial-gradient(ellipse at 50% 100%, rgba(255, 0, 0, 0.08) 0%, transparent 50%),
                linear-gradient(160deg, #180202 0%, #200505 30%, #180303 60%, #100101 100%);
              overflow: hidden;
              font-family: 'Poppins', sans-serif;
            }
            
            /* Grid pattern */
            .RKBM-wrapper::before {
              content: '';
              position: absolute;
              inset: 0;
              background-image:
                linear-gradient(rgba(255, 0, 0, 0.025) 1px, transparent 1px),
                linear-gradient(90deg, rgba(255, 0, 0, 0.025) 1px, transparent 1px);
              background-size: 55px 55px;
              pointer-events: none;
              z-index: 0;
            }
            
            /* ============================================
               PARTICLES
            ============================================ */
            .particle-wrap {
              position: absolute;
              inset: 0;
              pointer-events: none;
              overflow: hidden;
              z-index: 0;
            }
            .ptcl {
              position: absolute;
              border-radius: 50%;
              background: rgba(255, 0, 0, 0.2);
              animation: particleDrift linear infinite;
            }
            .ptcl:nth-child(1)  { width:5px;  height:5px;  left:8%;   bottom:15%; animation-duration:9s;  animation-delay:0s;   }
            .ptcl:nth-child(2)  { width:3px;  height:3px;  left:22%;  bottom:8%;  animation-duration:11s; animation-delay:1.2s; }
            .ptcl:nth-child(3)  { width:7px;  height:7px;  left:38%;  bottom:25%; animation-duration:8s;  animation-delay:2.5s; }
            .ptcl:nth-child(4)  { width:4px;  height:4px;  left:55%;  bottom:12%; animation-duration:13s; animation-delay:0.8s; }
            .ptcl:nth-child(5)  { width:6px;  height:6px;  left:70%;  bottom:20%; animation-duration:10s; animation-delay:1.8s; }
            .ptcl:nth-child(6)  { width:3px;  height:3px;  left:85%;  bottom:8%;  animation-duration:12s; animation-delay:3.2s; }
            .ptcl:nth-child(7)  { width:5px;  height:5px;  left:15%;  bottom:45%; animation-duration:7s;  animation-delay:2s;   }
            .ptcl:nth-child(8)  { width:4px;  height:4px;  left:48%;  bottom:55%; animation-duration:15s; animation-delay:0.5s; }
            .ptcl:nth-child(9)  { width:6px;  height:6px;  left:92%;  bottom:35%; animation-duration:9s;  animation-delay:4s;   }
            .ptcl:nth-child(10) { width:3px;  height:3px;  left:62%;  bottom:65%; animation-duration:11s; animation-delay:1.5s; }
            
            /* ============================================
               HERO SECTION
            ============================================ */
            .rkbm-hero {
              position: relative;
              z-index: 2;
              padding: 70px 24px 60px;
              text-align: center;
              border-bottom: 1px solid rgba(255, 0, 0, 0.08);
            }
            
            /* Top border glow */
            .rkbm-hero::before {
              content: '';
              position: absolute;
              top: 0; left: 0; right: 0;
              height: 2px;
              background: linear-gradient(90deg,
                transparent 0%,
                #00e1ff 20%,
                #ffffff 50%,
                #00e1ff 80%,
                transparent 100%
              );
              background-size: 200% 100%;
              animation: scanLine 4s linear infinite;
            }
            
            .rkbm-hero-badge {
              display: inline-flex;
              align-items: center;
              gap: 8px;
              padding: 7px 22px;
              background: linear-gradient(135deg,
                rgba(0,200,255,0.12),
                rgba(0,100,255,0.08)
              );
              border: 1px solid rgba(0,200,255,0.3);
              border-radius: 50px;
              font-family: 'Orbitron', sans-serif;
              font-size: 10px;
              font-weight: 700;
              letter-spacing: 3px;
              color: #00e1ff;
              text-transform: uppercase;
              margin-bottom: 20px;
              backdrop-filter: blur(10px);
              animation: fadeInUp 0.6s ease-out both;
            }
            
            .hero-badge-dot {
              width: 6px;
              height: 6px;
              border-radius: 50%;
              background: #00e1ff;
              box-shadow: 0 0 8px #00e1ff;
              animation: countBlink 1.5s ease-in-out infinite;
            }
            
            .rkbm-hero h1 {
              font-family: 'Orbitron', sans-serif;
              font-size: clamp(22px, 4vw, 42px);
              font-weight: 900;
              line-height: 1.25;
              margin-bottom: 20px;
              background: linear-gradient(135deg,
                #ffffff 0%,
                #00e1ff 25%,
                #7df9ff 50%,
                #00e1ff 75%,
                #ffffff 100%
              );
              background-size: 200% auto;
              -webkit-background-clip: text;
              -webkit-text-fill-color: transparent;
              background-clip: text;
              animation: shimmerText 5s linear infinite, fadeInUp 0.7s ease-out 0.1s both;
            }
            
            /* Garis dekorasi bawah judul */
            .hero-underline {
              display: flex;
              align-items: center;
              justify-content: center;
              gap: 12px;
              margin: 0 auto 28px;
              animation: fadeInUp 0.7s ease-out 0.2s both;
            }
            .hero-underline-line {
              height: 2px;
              border-radius: 2px;
              background: linear-gradient(90deg, transparent, #00e1ff, transparent);
              animation: lineExpand 1s ease-out 0.5s both;
              width: 80px;
            }
            .hero-underline-dot {
              width: 8px; height: 8px;
              border-radius: 50%;
              background: #00e1ff;
              box-shadow: 0 0 12px #00e1ff;
              animation: glowPulse 2s ease-in-out infinite;
            }
            
            .rkbm-hero-desc {
              font-size: clamp(14px, 2vw, 17px);
              color: rgba(255,255,255,0.72);
              max-width: 820px;
              margin: 0 auto 36px;
              line-height: 1.85;
              animation: fadeInUp 0.7s ease-out 0.3s both;
            }
            
            /* ============================================
               FEATURE CHIPS
            ============================================ */
            .hero-chips {
              display: flex;
              flex-wrap: wrap;
              justify-content: center;
              gap: 10px;
              margin-bottom: 40px;
              animation: fadeInUp 0.7s ease-out 0.4s both;
            }
            .hero-chip {
              display: inline-flex;
              align-items: center;
              gap: 6px;
              padding: 8px 18px;
              background: rgba(0,200,255,0.07);
              border: 1px solid rgba(255, 0, 0, 0.2);
              border-radius: 50px;
              font-size: 12px;
              font-weight: 600;
              color: rgba(255,255,255,0.75);
              letter-spacing: 0.5px;
              transition: all 0.3s ease;
              cursor: default;
            }
            .hero-chip:hover {
              background: rgba(0,200,255,0.15);
              border-color: rgba(0,200,255,0.5);
              color: #00e1ff;
              transform: translateY(-2px);
              box-shadow: 0 4px 15px rgba(255, 0, 0, 0.2);
            }
            .hero-chip-icon { font-size: 14px; }
            
            /* ============================================
               CONTENT PARAGRAPHS SECTION
            ============================================ */
            .RKBM-content {
              position: relative;
              z-index: 2;
              padding: 60px 24px;
              max-width: 1100px;
              margin: 0 auto;
            }
            
            .RKBM-content-grid {
              display: grid;
              grid-template-columns: 1fr 1fr;
              gap: 20px;
              margin-bottom: 20px;
            }
            
            .RKBM-content-full {
              grid-column: 1 / -1;
            }
            
            /* Content Card */
            .content-card {
              position: relative;
              background: rgba(255,255,255,0.025);
              border: 1px solid rgba(0,200,255,0.1);
              border-radius: 18px;
              padding: 28px 30px;
              transition: all 0.4s ease;
              overflow: hidden;
              backdrop-filter: blur(8px);
            }
            
            .content-card::before {
              content: '';
              position: absolute;
              top: 0; left: 0; right: 0;
              height: 2px;
              background: linear-gradient(90deg,
                transparent,
                rgba(0,200,255,0.5),
                transparent
              );
              opacity: 0;
              transition: opacity 0.3s ease;
            }
            
            .content-card:hover::before { opacity: 1; }
            
            .content-card:hover {
              background: rgba(0,200,255,0.05);
              border-color: rgba(255, 0, 0, 0.25);
              transform: translateY(-4px);
              box-shadow:
                0 12px 35px rgba(0,0,0,0.3),
                0 0 0 1px rgba(255, 0, 0, 0.08),
                inset 0 1px 0 rgba(255,255,255,0.04);
            }
            
            /* Left accent */
            .content-card::after {
              content: '';
              position: absolute;
              left: 0; top: 20%; bottom: 20%;
              width: 3px;
              background: linear-gradient(180deg, #00e1ff, #0066ff);
              border-radius: 0 3px 3px 0;
              opacity: 0;
              transition: opacity 0.3s ease;
            }
            .content-card:hover::after { opacity:1; }
            
            .content-card-icon {
              font-size: 28px;
              margin-bottom: 12px;
              display: block;
              animation: floatUp 3s ease-in-out infinite;
            }
            
            .content-card-title {
              font-family: 'Rajdhani', sans-serif;
              font-size: 17px;
              font-weight: 700;
              color: #00e1ff;
              margin-bottom: 10px;
              letter-spacing: 0.5px;
            }
            
            .content-card-text {
              font-size: 14px;
              color: rgba(255,255,255,0.65);
              line-height: 1.85;
              margin: 0;
            }
            
            /* ============================================
               STATS BAR
            ============================================ */
            .rkbm-stats {
              position: relative;
              z-index: 2;
              padding: 50px 24px;
              background: rgba(0,200,255,0.03);
              border-top: 1px solid rgba(0,200,255,0.07);
              border-bottom: 1px solid rgba(0,200,255,0.07);
            }
            
            .stats-inner {
              max-width: 1000px;
              margin: 0 auto;
              display: grid;
              grid-template-columns: repeat(4, 1fr);
              gap: 20px;
            }
            
            .stat-item {
              text-align: center;
              padding: 24px 16px;
              background: rgba(255,255,255,0.02);
              border: 1px solid rgba(0,200,255,0.1);
              border-radius: 16px;
              transition: all 0.3s ease;
              position: relative;
              overflow: hidden;
            }
            
            .stat-item::before {
              content: '';
              position: absolute;
              bottom: 0; left: 0; right: 0;
              height: 2px;
              background: linear-gradient(90deg, transparent, #00e1ff, transparent);
              transform: scaleX(0);
              transition: transform 0.3s ease;
            }
            
            .stat-item:hover::before { transform: scaleX(1); }
            
            .stat-item:hover {
              background: rgba(0,200,255,0.06);
              border-color: rgba(0,200,255,0.3);
              transform: translateY(-5px);
              box-shadow: 0 10px 30px rgba(0,200,255,0.15);
            }
            
            .stat-icon {
              font-size: 28px;
              margin-bottom: 8px;
              display: block;
            }
            
            .stat-value {
              font-family: 'Orbitron', sans-serif;
              font-size: 28px;
              font-weight: 900;
              background: linear-gradient(135deg, #00e1ff, #0099ff);
              -webkit-background-clip: text;
              -webkit-text-fill-color: transparent;
              background-clip: text;
              line-height: 1;
              margin-bottom: 6px;
            }
            
            .stat-label {
              font-family: 'Rajdhani', sans-serif;
              font-size: 12px;
              font-weight: 600;
              color: rgba(255,255,255,0.45);
              letter-spacing: 1.5px;
              text-transform: uppercase;
            }
            
            /* ============================================
               KALAU INI BUAT FAQ YAAA 
            ============================================ */
            .rkbm-faq {
              position: relative;
              z-index: 2;
              padding: 80px 24px 90px;
              max-width: 1000px;
              margin: 0 auto;
            }
            
            .section-title-wrap {
              text-align: center;
              margin-bottom: 55px;
              animation: fadeInUp 0.7s ease-out both;
            }
            
            .section-badge {
              display: inline-flex;
              align-items: center;
              gap: 8px;
              padding: 7px 22px;
              background: linear-gradient(135deg,
                rgba(0,200,255,0.12),
                rgba(0,100,255,0.08)
              );
              border: 1px solid rgba(0,200,255,0.3);
              border-radius: 50px;
              font-family: 'Orbitron', sans-serif;
              font-size: 10px;
              font-weight: 700;
              letter-spacing: 3px;
              color: #00e1ff;
              text-transform: uppercase;
              margin-bottom: 18px;
              backdrop-filter: blur(10px);
            }
            
            .section-title {
              font-family: 'Orbitron', sans-serif;
              font-size: clamp(22px, 3.5vw, 36px);
              font-weight: 900;
              background: linear-gradient(135deg,
                #ffffff 0%,
                #00e1ff 30%,
                #7df9ff 50%,
                #00e1ff 70%,
                #ffffff 100%
              );
              background-size: 200% auto;
              -webkit-background-clip: text;
              -webkit-text-fill-color: transparent;
              background-clip: text;
              animation: shimmerText 5s linear infinite;
              margin-bottom: 14px;
              line-height: 1.3;
            }
            
            .section-underline {
              display: flex;
              align-items: center;
              justify-content: center;
              gap: 12px;
              margin-top: 14px;
            }
            .section-underline-line {
              height: 2px;
              width: 70px;
              border-radius: 2px;
              background: linear-gradient(90deg, transparent, #00e1ff, transparent);
            }
            .section-underline-dot {
              width: 8px; height: 8px;
              border-radius: 50%;
              background: #00e1ff;
              box-shadow: 0 0 10px #00e1ff;
              animation: glowPulse 2s ease-in-out infinite;
            }
            
            /* FAQ Items */
            .faq-list {
              display: flex;
              flex-direction: column;
              gap: 14px;
            }
            
            .faq-item-new {
              position: relative;
              background: rgba(255,255,255,0.025);
              border: 1px solid rgba(0,200,255,0.1);
              border-radius: 16px;
              overflow: hidden;
              transition: all 0.4s ease;
              animation: fadeInUp 0.6s ease-out both;
            }
            
            .faq-item-new:nth-child(1)  { animation-delay: 0.05s; }
            .faq-item-new:nth-child(2)  { animation-delay: 0.10s; }
            .faq-item-new:nth-child(3)  { animation-delay: 0.15s; }
            .faq-item-new:nth-child(4)  { animation-delay: 0.20s; }
            .faq-item-new:nth-child(5)  { animation-delay: 0.25s; }
            .faq-item-new:nth-child(6)  { animation-delay: 0.30s; }
            .faq-item-new:nth-child(7)  { animation-delay: 0.35s; }
            .faq-item-new:nth-child(8)  { animation-delay: 0.40s; }
            .faq-item-new:nth-child(9)  { animation-delay: 0.45s; }
            .faq-item-new:nth-child(10) { animation-delay: 0.50s; }
            
            .faq-item-new.faq-open {
              background: rgba(0,200,255,0.05);
              border-color: rgba(0,200,255,0.3);
              box-shadow:
                0 8px 30px rgba(0,0,0,0.3),
                0 0 0 1px rgba(255, 0, 0, 0.08),
                inset 0 1px 0 rgba(255,255,255,0.04);
            }
            
            /* Left accent bar */
            .faq-item-new::before {
              content: '';
              position: absolute;
              left: 0; top: 0; bottom: 0;
              width: 3px;
              background: linear-gradient(180deg, #00e1ff, #0066ff);
              border-radius: 3px 0 0 3px;
              opacity: 0;
              transition: opacity 0.3s ease;
            }
            .faq-item-new.faq-open::before { opacity: 1; }
            
            /* FAQ Question Button */
            .faq-btn-new {
              width: 100%;
              padding: 22px 28px;
              background: transparent;
              border: none;
              cursor: pointer;
              display: flex;
              justify-content: space-between;
              align-items: center;
              gap: 16px;
              text-align: left;
              transition: all 0.3s ease;
            }
            
            .faq-btn-new:hover { background: rgba(0,200,255,0.03); }
            
            .faq-num {
              flex-shrink: 0;
              width: 34px;
              height: 34px;
              border-radius: 50%;
              background: rgba(0,200,255,0.1);
              border: 1px solid rgba(255, 0, 0, 0.25);
              display: flex;
              align-items: center;
              justify-content: center;
              font-family: 'Orbitron', sans-serif;
              font-size: 11px;
              font-weight: 700;
              color: #00e1ff;
              transition: all 0.3s ease;
            }
            
            .faq-item-new.faq-open .faq-num {
              background: linear-gradient(135deg, #00e1ff, #0066ff);
              color: #000;
              border-color: transparent;
              box-shadow: 0 0 12px rgba(0,200,255,0.5);
            }
            
            .faq-question-text {
              flex: 1;
              font-family: 'Poppins', sans-serif;
              font-size: 15px;
              font-weight: 600;
              color: rgba(255,255,255,0.85);
              line-height: 1.5;
              transition: color 0.3s ease;
            }
            
            .faq-item-new.faq-open .faq-question-text,
            .faq-btn-new:hover .faq-question-text {
              color: #ffffff;
            }
            
            .faq-toggle-icon {
              flex-shrink: 0;
              width: 34px;
              height: 34px;
              border-radius: 50%;
              background: rgba(255, 0, 0, 0.08);
              border: 1px solid rgba(255, 0, 0, 0.2);
              display: flex;
              align-items: center;
              justify-content: center;
              font-size: 18px;
              color: #00e1ff;
              font-weight: 300;
              transition: all 0.4s cubic-bezier(0.34,1.56,0.64,1);
            }
            
            .faq-item-new.faq-open .faq-toggle-icon {
              transform: rotate(135deg);
              background: linear-gradient(135deg, #00e1ff, #0066ff);
              color: #000;
              border-color: transparent;
              box-shadow: 0 0 12px rgba(0,200,255,0.4);
            }
            
            /* FAQ Answer */
            .faq-answer-new {
              max-height: 0;
              overflow: hidden;
              transition: max-height 0.5s ease, padding 0.4s ease;
              padding: 0 28px 0 28px;
            }
            
            .faq-item-new.faq-open .faq-answer-new {
              max-height: 600px;
              padding: 0 28px 24px 76px;
            }
            
            .faq-answer-new p {
              font-family: 'Poppins', sans-serif;
              font-size: 14px;
              color: rgba(255,255,255,0.6);
              line-height: 1.9;
              margin: 0;
              border-top: 1px solid rgba(0,200,255,0.1);
              padding-top: 16px;
            }
            
            /* ============================================
               TESTI NYA KAKAK
            ============================================ */
            .rkbm-testimoni {
              position: relative;
              z-index: 2;
              padding: 80px 24px 90px;
              background:
                radial-gradient(ellipse at 50% 0%, rgba(0,150,255,0.08) 0%, transparent 60%),
                rgba(0,0,0,0.2);
              border-top: 1px solid rgba(0,200,255,0.07);
            }
            
            .testimoni-inner {
              max-width: 1200px;
              margin: 0 auto;
            }
            
            /* Grid Testimoni */
            .testi-grid {
              display: grid;
              grid-template-columns: repeat(3, 1fr);
              gap: 20px;
              margin-bottom: 50px;
            }
            
            /* Testimoni Card */
            .testi-card {
              position: relative;
              background: rgba(255,255,255,0.025);
              border: 1px solid rgba(0,200,255,0.1);
              border-radius: 20px;
              padding: 28px 26px;
              transition: all 0.4s cubic-bezier(0.34,1.56,0.64,1);
              overflow: hidden;
              animation: cardEntrance 0.6s ease-out both;
            }
            
            .testi-card:nth-child(1)  { animation-delay: 0.05s; }
            .testi-card:nth-child(2)  { animation-delay: 0.10s; }
            .testi-card:nth-child(3)  { animation-delay: 0.15s; }
            .testi-card:nth-child(4)  { animation-delay: 0.20s; }
            .testi-card:nth-child(5)  { animation-delay: 0.25s; }
            .testi-card:nth-child(6)  { animation-delay: 0.30s; }
            .testi-card:nth-child(7)  { animation-delay: 0.35s; }
            .testi-card:nth-child(8)  { animation-delay: 0.40s; }
            .testi-card:nth-child(9)  { animation-delay: 0.45s; }
            .testi-card:nth-child(10) { animation-delay: 0.50s; }
            
            /* Shine overlay */
            .testi-card::before {
              content: '';
              position: absolute;
              top: -50%; left: -60%;
              width: 220%; height: 200%;
              background: radial-gradient(
                circle,
                rgba(0,200,255,0.06) 0%,
                transparent 65%
              );
              transition: opacity 0.4s ease;
              opacity: 0;
              pointer-events: none;
            }
            
            .testi-card:hover::before { opacity: 1; }
            
            .testi-card:hover {
              background: rgba(0,200,255,0.06);
              border-color: rgba(0,200,255,0.3);
              transform: translateY(-8px) scale(1.01);
              box-shadow:
                0 20px 50px rgba(0,0,0,0.4),
                0 0 0 1px rgba(0,200,255,0.1),    inset 0 1px 0 rgba(255,255,255,0.05);
              }
              
              /* Top accent line */
              .testi-card::after {
                content: '';
                position: absolute;
                top: 0; left: 10%; right: 10%;
                height: 2px;
                background: linear-gradient(90deg, transparent, #00e1ff, transparent);
                border-radius: 2px;
                opacity: 0;
                transition: opacity 0.3s ease;
              }
              .testi-card:hover::after { opacity: 1; }
              
              /* Quote icon */
              .testi-quote-icon {
                font-size: 40px;
                line-height: 1;
                color: rgba(255, 0, 0, 0.2);
                font-family: Georgia, serif;
                margin-bottom: 8px;
                display: block;
                transition: color 0.3s ease;
              }
              .testi-card:hover .testi-quote-icon {
                color: rgba(0,200,255,0.45);
              }
              
              /* Stars */
              .testi-stars {
                display: flex;
                gap: 3px;
                margin-bottom: 14px;
              }
              .testi-star {
                font-size: 16px;
                animation: starPop 0.4s ease-out both;
              }
              .testi-star:nth-child(1) { animation-delay: 0.05s; }
              .testi-star:nth-child(2) { animation-delay: 0.10s; }
              .testi-star:nth-child(3) { animation-delay: 0.15s; }
              .testi-star:nth-child(4) { animation-delay: 0.20s; }
              .testi-star:nth-child(5) { animation-delay: 0.25s; }
              
              /* Quote text */
              .testi-text {
                font-family: 'Poppins', sans-serif;
                font-size: 13.5px;
                color: rgba(255,255,255,0.7);
                line-height: 1.85;
                font-style: italic;
                margin-bottom: 20px;
                flex: 1;
              }
              
              /* Author */
              .testi-author {
                display: flex;
                align-items: center;
                gap: 12px;
                padding-top: 16px;
                border-top: 1px solid rgba(255, 0, 0, 0.08);
              }
              
              .testi-avatar {
                width: 40px;
                height: 40px;
                border-radius: 50%;
                background: linear-gradient(135deg, #00e1ff, #0066ff);
                display: flex;
                align-items: center;
                justify-content: center;
                font-family: 'Orbitron', sans-serif;
                font-size: 14px;
                font-weight: 700;
                color: #000;
                flex-shrink: 0;
                box-shadow: 0 0 12px rgba(0,200,255,0.4);
                transition: all 0.3s ease;
              }
              .testi-card:hover .testi-avatar {
                box-shadow: 0 0 20px rgba(0,200,255,0.7);
                transform: scale(1.08);
              }
              
              .testi-author-info { flex: 1; }
              
              .testi-author-name {
                font-family: 'Rajdhani', sans-serif;
                font-size: 14px;
                font-weight: 700;
                color: #ffffff;
                letter-spacing: 0.3px;
                display: block;
              }
              
              .testi-author-meta {
                display: flex;
                align-items: center;
                gap: 6px;
                margin-top: 2px;
              }
              
              .testi-author-city {
                font-size: 11px;
                color: rgba(255,255,255,0.4);
                font-family: 'Poppins', sans-serif;
              }
              
              .testi-author-time {
                font-size: 10px;
                color: rgba(0,200,255,0.5);
                font-family: 'Orbitron', sans-serif;
                letter-spacing: 0.5px;
              }
              
              .testi-author-sep {
                width: 3px;
                height: 3px;
                border-radius: 50%;
                background: rgba(255,255,255,0.2);
              }
              
              /* Verified badge */
              .testi-verified {
                display: inline-flex;
                align-items: center;
                gap: 4px;
                padding: 3px 9px;
                background: rgba(0,255,136,0.08);
                border: 1px solid rgba(0,255,136,0.2);
                border-radius: 50px;
                font-size: 9px;
                font-weight: 700;
                font-family: 'Orbitron', sans-serif;
                color: #00ff88;
                letter-spacing: 0.5px;
              }
              .testi-verified-dot {
                width: 5px; height: 5px;
                border-radius: 50%;
                background: #00ff88;
                box-shadow: 0 0 5px #00ff88;
                animation: countBlink 1.5s ease-in-out infinite;
              }
              
              /* ============================================
                 TESTIMONI CLOSING
              ============================================ */
              .testi-closing-wrap {
                position: relative;
                max-width: 860px;
                margin: 0 auto;
                padding: 36px 40px;
                background: rgba(0,200,255,0.04);
                border: 1px solid rgba(0,200,255,0.15);
                border-radius: 20px;
                text-align: center;
                overflow: hidden;
                animation: fadeInUp 0.7s ease-out 0.5s both;
              }
              
              .testi-closing-wrap::before {
                content: '';
                position: absolute;
                top: 0; left: 0; right: 0;
                height: 2px;
                background: linear-gradient(90deg,
                  transparent, #00e1ff, #ffffff, #00e1ff, transparent
                );
                background-size: 200% 100%;
                animation: scanLine 4s linear infinite;
              }
              
              .testi-closing-icon {
                font-size: 32px;
                margin-bottom: 14px;
                display: block;
                animation: floatUp 3s ease-in-out infinite;
              }
              
              .testi-closing-text {
                font-family: 'Poppins', sans-serif;
                font-size: 15px;
                color: rgba(255,255,255,0.65);
                line-height: 1.9;
                font-style: italic;
                margin: 0;
              }
              
              .testi-closing-text strong {
                color: #00e1ff;
                font-style: normal;
              }
              
              /* ============================================
                 CTA SECTION
              ============================================ */
              .rkbm-cta {
                position: relative;
                z-index: 2;
                padding: 70px 24px 80px;
                text-align: center;
                border-top: 1px solid rgba(0,200,255,0.07);
              }
              
              .cta-title {
                font-family: 'Orbitron', sans-serif;
                font-size: clamp(20px, 3vw, 32px);
                font-weight: 900;
                color: #ffffff;
                margin-bottom: 14px;
                animation: fadeInUp 0.6s ease-out both;
              }
              
              .cta-subtitle {
                font-size: 15px;
                color: rgba(255,255,255,0.55);
                margin-bottom: 36px;
                font-family: 'Poppins', sans-serif;
                animation: fadeInUp 0.6s ease-out 0.1s both;
              }
              
              .cta-buttons {
                display: flex;
                justify-content: center;
                gap: 16px;
                flex-wrap: wrap;
                animation: fadeInUp 0.6s ease-out 0.2s both;
              }
              
              .cta-btn-primary {
                display: inline-flex;
                align-items: center;
                gap: 10px;
                padding: 16px 44px;
                font-family: 'Orbitron', sans-serif;
                font-size: 13px;
                font-weight: 700;
                letter-spacing: 2px;
                text-decoration: none;
                color: #000;
                border-radius: 50px;
                position: relative;
                overflow: hidden;
                transition: all 0.3s ease;
                background: linear-gradient(135deg,
                  #00aaff 0%,
                  #00e1ff 30%,
                  #7df9ff 50%,
                  #00e1ff 70%,
                  #00aaff 100%
                );
                background-size: 200% auto;
                animation: shimmerText 3s linear infinite;
                box-shadow:
                  0 0 20px rgba(0,200,255,0.4),
                  0 8px 25px rgba(0,150,255,0.3),
                  inset 0 1px 0 rgba(255,255,255,0.4);
              }
              
              .cta-btn-primary::before {
                content: '';
                position: absolute;
                inset: 2px;
                border-radius: 48px;
                background: linear-gradient(135deg,
                  rgba(255,255,255,0.25) 0%,
                  transparent 50%
                );
                pointer-events: none;
              }
              
              .cta-btn-primary:hover {
                transform: translateY(-3px) scale(1.03);
                box-shadow:
                  0 0 40px rgba(0,200,255,0.7),
                  0 15px 35px rgba(0,150,255,0.5),
                  inset 0 1px 0 rgba(255,255,255,0.5);
              }
              
              .cta-btn-secondary {
                display: inline-flex;
                align-items: center;
                gap: 10px;
                padding: 16px 44px;
                font-family: 'Orbitron', sans-serif;
                font-size: 13px;
                font-weight: 700;
                letter-spacing: 2px;
                text-decoration: none;
                color: #00e1ff;
                border-radius: 50px;
                border: 2px solid rgba(0,200,255,0.4);
                background: rgba(0,200,255,0.06);
                transition: all 0.3s ease;
                backdrop-filter: blur(10px);
              }
              
              .cta-btn-secondary:hover {
                background: rgba(0,200,255,0.15);
                border-color: rgba(0,200,255,0.7);
                transform: translateY(-3px);
                box-shadow: 0 8px 25px rgba(255, 0, 0, 0.2);
                color: #ffffff;
              }
              
              /* ============================================
                 RESPONSIVE
              ============================================ */
              @media (max-width: 1024px) {
                .testi-grid {
                  grid-template-columns: repeat(2, 1fr);
                }
                .stats-inner {
                  grid-template-columns: repeat(2, 1fr);
                }
              }
              
              @media (max-width: 768px) {
                .rkbm-hero { padding: 55px 18px 50px; }
                .RKBM-content { padding: 45px 18px; }
                .rkbm-faq { padding: 55px 18px 65px; }
                .rkbm-testimoni { padding: 55px 18px 65px; }
                .rkbm-cta { padding: 55px 18px 65px; }
              
                .RKBM-content-grid {
                  grid-template-columns: 1fr;
                }
              
                .testi-grid {
                  grid-template-columns: 1fr;
                  gap: 16px;
                }
              
                .stats-inner {
                  grid-template-columns: repeat(2, 1fr);
                  gap: 14px;
                }
              
                .stat-value { font-size: 22px; }
              
                .faq-btn-new { padding: 18px 20px; }
                .faq-item-new.faq-open .faq-answer-new {
                  padding: 0 20px 20px 20px;
                }
              
                .testi-closing-wrap { padding: 28px 22px; }
              
                .cta-buttons { flex-direction: column; align-items: center; }
                .cta-btn-primary,
                .cta-btn-secondary { width: 100%; max-width: 320px; justify-content: center; }
              }
              
              @media (max-width: 480px) {
                .rkbm-hero h1 { font-size: 20px; }
                .section-title { font-size: 20px; }
                .hero-chips { gap: 7px; }
                .hero-chip { font-size: 11px; padding: 6px 13px; }
                .stats-inner { grid-template-columns: repeat(2, 1fr); gap: 10px; }
                .stat-item { padding: 18px 10px; }
                .stat-value { font-size: 20px; }
                .faq-question-text { font-size: 13px; }
                .testi-closing-text { font-size: 13px; }
              }
              
              </style>
              
              <!-- ============================================
                   HTML STRUKTUR LENGKAP
              ============================================ -->
              <div class="RKBM-wrapper">
              
                <!-- Particles -->
                <div class="particle-wrap">
                  <div class="ptcl"></div><div class="ptcl"></div>
                  <div class="ptcl"></div><div class="ptcl"></div>
                  <div class="ptcl"></div><div class="ptcl"></div>
                  <div class="ptcl"></div><div class="ptcl"></div>
                  <div class="ptcl"></div><div class="ptcl"></div>
                </div>
              
                <!-- ==================== HERO ==================== -->
                <div class="rkbm-hero">
                  <div class="rkbm-hero-badge">
                    <span class="hero-badge-dot"></span>
                    ✦ PLATFORM TERPERCAYA ✦
                  </div>
              
                  <h1>Ai Mr Sultan 🛩️ Bandar Situs Judi Slot Online Gacor & Link Slot88 Jackpot Terbesar</h1>
               - 
                  <div class="hero-underline">
                    <div class="hero-underline-line"></div>
                    <div class="hero-underline-dot"></div>
                    <div class="hero-underline-line"></div>
                  </div>
              
                  <p class="rkbm-hero-desc">
                    Judi Slot 88 gacor datang sebagai link slot online terbaik bagi pecinta game slot online yang memiliki sistem keamanan paling update dan nyaman dari segi manapun, pengguna bisa merasakan sensasi kemenangan jackpot maxwin termudah hanya dalam beberapa kali putaran mesin slot saja. Ai Mr Sultan telah diakui penjuru asia tenggara yang sangat gemar bermain game judi slot online!
                  </p>

                  <div class="hero-chips">
                    <div class="hero-chip"><span class="hero-chip-icon">⚡</span> Server Cepat</div>
                    <div class="hero-chip"><span class="hero-chip-icon">🔒</span> Sistem Aman</div>
                    <div class="hero-chip"><span class="hero-chip-icon">🎰</span> Slot Gacor</div>
                    <div class="hero-chip"><span class="hero-chip-icon">💎</span> RTP Tinggi</div>
                    <div class="hero-chip"><span class="hero-chip-icon">🏆</span> Judi Slot</div>
                    <div class="hero-chip"><span class="hero-chip-icon">📱</span> Mobile Friendly</div>
                    <div class="hero-chip"><span class="hero-chip-icon">🌏</span> Asia Tenggara</div>
                    <div class="hero-chip"><span class="hero-chip-icon">⏰</span> 24 Jam Aktif</div>
                  </div>
                </div>
              
                <!-- ==================== GARRRR ==================== -->
                <div class="rkbm-stats">
                  <div class="stats-inner">
                    <div class="stat-item">
                      <span class="stat-icon">👥</span>
                      <div class="stat-value" data-count="500">500K+</div>
                      <div class="stat-label">Member Aktif</div>
                    </div>
                    <div class="stat-item">
                      <span class="stat-icon">🎮</span>
                      <div class="stat-value" data-count="1000">1000+</div>
                      <div class="stat-label">Game Tersedia</div>
                    </div>
                    <div class="stat-item">
                      <span class="stat-icon">⚡</span>
                      <div class="stat-value" data-count="99">99%</div>
                      <div class="stat-label">Uptime Server</div>
                    </div>
                    <div class="stat-item">
                      <span class="stat-icon">🏅</span>
                      <div class="stat-value" data-count="24">24/7</div>
                      <div class="stat-label">Layanan CS</div>
                    </div>
                  </div>
                </div>
              
                <!-- ==================== BANG BUDDDD ==================== -->
                <div class="RKBM-content">
              
                  <!-- Row 1: 2 kolom -->
                  <div class="RKBM-content-grid">
                    
                    <div class="content-card">
                      <span class="content-card-icon">🎰</span>
                      <div class="content-card-title">Koleksi Game Slot Terlengkap</div>
                      <p class="content-card-text">
                        AI MR SULTAN menyediakan beragam pilihan permainan slot terbaik dari provider
                        ternama seperti Pragmatic Play, PG Soft, Habanero, hingga Microgaming.
                        Setiap game telah dikurasi dengan RTP tinggi dan sistem fair play, sehingga
                        pemain dapat merasakan pengalaman bermain yang transparan dan menguntungkan.
                      </p>
                    </div>

                    <div class="content-card">
                      <span class="content-card-icon">📱</span>
                      <div class="content-card-title">Akses Mudah Mobile Friendly</div>
                      <p class="content-card-text">
                        Keunggulan utama dari link AI MR SULTAN adalah kemudahan akses yang dapat
                        digunakan kapan saja dan di mana saja. Dengan tampilan mobile-friendly,
                        pemain bisa bermain hanya melalui smartphone tanpa harus menggunakan
                        perangkat tambahan. Sistem login yang cepat dan link alternatif yang selalu
                        update memastikan pengguna tetap bisa masuk tanpa hambatan.
                      </p>
                    </div>

                    <div class="content-card">
                      <span class="content-card-icon">🌐</span>
                      <div class="content-card-title">Server Asia Tenggara Tercepat</div>
                      <p class="content-card-text">
                        Dengan dukungan server Asia Tenggara yang terkenal cepat dan minim gangguan,
                        pemain dapat menikmati akses tanpa lag saat bermain berbagai game slot favorit.
                        Hal ini sangat penting terutama saat berburu momen "gacor" di game slot
                        yang membutuhkan koneksi stabil untuk memaksimalkan peluang kemenangan.
                      </p>
                    </div>

                    <div class="content-card">
                      <span class="content-card-icon">🔒</span>
                      <div class="content-card-title">Keamanan Sistem Enkripsi Modern</div>
                      <p class="content-card-text">
                        AI MR SULTAN menggunakan sistem enkripsi modern untuk melindungi data dan
                        transaksi pemain. Semua proses deposit dan withdraw dilakukan secara cepat
                        dan aman, sehingga pemain tidak perlu khawatir terhadap keamanan dana mereka.
                        Privasi dan keamanan Anda adalah prioritas utama kami.
                      </p>
                    </div>
              
                  </div>
              
                  <!-- Row 2: Full width -->
                  <div class="RKBM-content-grid">
                    <div class="content-card RKBM-content-full">
                      <span class="content-card-icon">🏆</span>
                      <div class="content-card-title">Mengapa AI MR SULTAN Menjadi Pilihan Utama?</div>
                      <p class="content-card-text">
                        Tidak ada lagi situs judi slot lain yang berani mengeluarkan JP maxwin setiap hari sampai ratusan juta sampai miliaran rupiah di seluruh penjuru negara asia, terutama di Indonesia hanya situs Ai Mr Sultan yang berani memberikan link judi slot online gampang maxwin terbaru demi kepuasan hati dari setiap member setia kami maupun akun baru pada situs slot kami.
                      </p>
                    </div>
                  </div>
              
                </div>
              
                <!-- ==================== FAQ ==================== -->
                <div class="rkbm-faq">
              
                  <div class="section-title-wrap">
                    <div class="section-badge">
                      <span class="hero-badge-dot"></span>
                      ✦ FAQ ✦
                    </div>
                    <div class="section-title">Pertanyaan - Pertanyaan Gacor Hari Ini</div>
                    <div class="section-underline">
                      <div class="section-underline-line"></div>
                      <div class="section-underline-dot"></div>
                      <div class="section-underline-line"></div>
                    </div>
                  </div>
              
                  <div class="faq-list">
              
                    <!-- FAQ 1 -->
                    <div class="faq-item-new">
                      <button class="faq-btn-new">
                        <span class="faq-num">01</span>
                        <span class="faq-question-text">Apa itu Ai Mr Sultan, mengapa bermain disini?</span>
                        <span class="faq-toggle-icon">+</span>
                      </button>
                      <div class="faq-answer-new">
                        <p>Ai Mr Sultan adalah situs penyedia permainan judi online baru terpercaya dan resmi yang berlisensi. kami menyediakan link slot gacor gampang menang direkomendasikan agen slot88 sebagai permainan slot online anti kalah peluang JP maxwin paling besar.</p>
                      </div>
                    </div>
              
                    <!-- FAQ 2 -->
                    <div class="faq-item-new">
                      <button class="faq-btn-new">
                        <span class="faq-num">02</span>
                        <span class="faq-question-text">Berapa Depo Terkecil Judi Slot Online?</span>
                        <span class="faq-toggle-icon">+</span>
                      </button>
                      <div class="faq-answer-new">
                        <p>Minimal depo judi slot online mulai dari 10 ribu rupiah, langsung bisa akses semua game slot.</p>
                      </div>
                    </div>
              
                    <!-- FAQ 3 -->
                    <div class="faq-item-new">
                      <button class="faq-btn-new">
                        <span class="faq-num">03</span>
                        <span class="faq-question-text">Apa Saja Bonus Harian Situs Nike Slot 88?</span>
                        <span class="faq-toggle-icon">+</span>
                      </button>
                      <div class="faq-answer-new">
                        <p>Terdapat Bonus depo setiap hari yang dapat di claim kapanpun, bonus mingguan juga bisa dilihat pada halaman pengumuman.</p>
                      </div>
                    </div>
              
                    <!-- FAQ 4 -->
                    <div class="faq-item-new">
                      <button class="faq-btn-new">
                        <span class="faq-num">04</span>
                        <span class="faq-question-text">Kapan Palayanan Situs Judi Slot Tersedia?</span>
                        <span class="faq-toggle-icon">+</span>
                      </button>
                      <div class="faq-answer-new">
                        <p>Situs slot gampang menang memiliki pelayanan pelanggan setiap waktu 24/7 tanpa gangguan. Anda bisa hubungi tim kami mengenai kendala permainan slot online sampai masalah seputar perjudian lainnya.</p>
                      </div>
                    </div>
              
                    <!-- FAQ 5 -->
                    <div class="faq-item-new">
                      <button class="faq-btn-new">
                        <span class="faq-num">05</span>
                        <span class="faq-question-text">Apa Tips Main Slot Online JP Maxwin?</span>
                        <span class="faq-toggle-icon">+</span>
                      </button>
                      <div class="faq-answer-new">
                        <p>Ai Mr Sultan secara rutin menawarkan berbagai pola dan jam gacor yang bisa jadi pedoman member judi online, manfaatkan sebaik-baiknya, dan jangan pernah lewatkan peluang jackpot anda di situs gacor nike slot 88.</p>
                      </div>
                    </div>
              
                    <!-- FAQ 6 -->
                    <div class="faq-item-new">
                      <button class="faq-btn-new">
                        <span class="faq-num">06</span>
                        <span class="faq-question-text">Apakah ada link alternatif Ai Mr Sultan?</span>
                        <span class="faq-toggle-icon">+</span>
                      </button>
                      <div class="faq-answer-new">
                        <p>Ya, Ai Mr Sultan menyediakan Platform link alternatif slot yang selalu aktif dan terhindar dari pemblokiran, maka dari itu anda harus selalu mencari situs yang paling update seperti kami.</p>
                      </div>
                    </div>
              
              
                  </div>
                </div>
              
                <!-- ==================== TESTIMONI ==================== -->
                <div class="rkbm-testimoni">
                  <div class="testimoni-inner">
              
                    <div class="section-title-wrap">
                      <div class="section-badge">
                        <span class="hero-badge-dot"></span>
                        ✦ TESTIMONI PARA DEWA SLOT GACOR ✦
                      </div>
                      <div class="section-title">Kesaksian Nyata dari Para Dewa Slot Gacor</div>
                      <div class="section-underline">
                        <div class="section-underline-line"></div>
                        <div class="section-underline-dot"></div>
                        <div class="section-underline-line"></div>
                      </div>
                    </div>
              
                    <div class="testi-grid">
              
                      <!-- Testi 1 -->
                      <div class="testi-card">
                        <span class="testi-quote-icon">"</span>
                        <div class="testi-stars">
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span             class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span>
                        </div>
                        <p class="testi-text">
                          "Saya udah coba beberapa situs slot, tapi yang paling gacor menurut saya itu situs yang punya RTP tinggi dan update setiap hari. Biasanya saya main di jam malam, dan hasilnya sering banget tembus scatter atau free spin. Situs slot gacor hari ini benar-benar bantu saya dapet cuan konsisten tanpa harus keluar modal besar."
                        </p>
                        <div class="testi-author">
                          <div class="testi-avatar">R</div>
                          <div class="testi-author-info">
                            <span class="testi-author-name">Raka Buming Gibran</span>
                            <div class="testi-author-meta">
                              <span class="testi-author-city">Jakarta</span>
                              <span class="testi-author-sep"></span>
                              <span class="testi-author-time">2 hari lalu</span>
                            </div>
                          </div>
                          <div class="testi-verified">
                            <span class="testi-verified-dot"></span>
                            VERIFIED
                          </div>
                        </div>
                      </div>
              
                      <!-- Testi 2 -->
                      <div class="testi-card">
                        <span class="testi-quote-icon">"</span>
                        <div class="testi-stars">
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span>
                        </div>
                        <p class="testi-text">
                          "Saya suka main di situs slot gacor karena mereka punya rekomendasi game yang lagi hot setiap harinya. Biasanya game pragmatic dan pgsoft lagi gacor banget. Dengan modal kecil, bisa dapet free spin berkali-kali."
                        </p>
                        <div class="testi-author">
                          <div class="testi-avatar">A</div>
                          <div class="testi-author-info">
                            <span class="testi-author-name">GAR GARING</span>
                            <div class="testi-author-meta">
                              <span class="testi-author-city">Bandung</span>
                              <span class="testi-author-sep"></span>
                              <span class="testi-author-time">3 hari lalu</span>
                            </div>
                          </div>
                          <div class="testi-verified">
                            <span class="testi-verified-dot"></span>
                            VERIFIED
                          </div>
                        </div>
                      </div>
              
                      <!-- Testi 3 -->
                      <div class="testi-card">
                        <span class="testi-quote-icon">"</span>
                        <div class="testi-stars">
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span>
                        </div>
                        <p class="testi-text">
                          "Situs slot gacor favorit saya selalu kasih info RTP live dan jam gacor tiap game. Info kayak gini penting banget buat tahu kapan waktu terbaik buat spin. Hasilnya, hampir tiap hari bisa dapet profit kecil tapi stabil."
                        </p>
                        <div class="testi-author">
                          <div class="testi-avatar">F</div>
                          <div class="testi-author-info">
                            <span class="testi-author-name">Bento Mujair</span>
                            <div class="testi-author-meta">
                              <span class="testi-author-city">Surabaya</span>
                              <span class="testi-author-sep"></span>
                              <span class="testi-author-time">4 hari lalu</span>
                            </div>
                          </div>
                          <div class="testi-verified">
                            <span class="testi-verified-dot"></span>
                            VERIFIED
                          </div>
                        </div>
                      </div>
              
                      <!-- Testi 4 -->
                      <div class="testi-card">
                        <span class="testi-quote-icon">"</span>
                        <div class="testi-stars">
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span>
                        </div>
                        <p class="testi-text">
                          "Awalnya saya ragu main slot online, tapi ternyata situs slot gacor yang saya temuin punya sistem keamanan bagus dan proses WD-nya cepet banget. Selain itu, update info slot gacor tiap hari bikin saya tahu game mana yang lagi gampang menang."
                        </p>
                        <div class="testi-author">
                          <div class="testi-avatar">D</div>
                          <div class="testi-author-info">
                            <span class="testi-author-name">Mario Naulana</span>
                            <div class="testi-author-meta">
                              <span class="testi-author-city">Medan</span>
                              <span class="testi-author-sep"></span>
                              <span class="testi-author-time">5 hari lalu</span>
                            </div>
                          </div>
                          <div class="testi-verified">
                            <span class="testi-verified-dot"></span>
                            VERIFIED
                          </div>
                        </div>
                      </div>
              
                      <!-- Testi 5 -->
                      <div class="testi-card">
                        <span class="testi-quote-icon">"</span>
                        <div class="testi-stars">
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span>
                        </div>
                        <p class="testi-text">
                          "Ai Mr Sultan sangat praktis bisa dimainkan melalui Aplikasi super gacor di link slot 777 deposit 1000 winrate 99% menang mudah."
                        </p>
                        <div class="testi-author">
                          <div class="testi-avatar">Y</div>
                          <div class="testi-author-info">
                            <span class="testi-author-name">Yogi Pranata</span>
                            <div class="testi-author-meta">
                              <span class="testi-author-city">Bekasi</span>
                              <span class="testi-author-sep"></span>
                              <span class="testi-author-time">6 hari lalu</span>
                            </div>
                          </div>
                          <div class="testi-verified">
                            <span class="testi-verified-dot"></span>
                            VERIFIED
                          </div>
                        </div>
                      </div>
              
                      <!-- Testi 6 -->
                      <div class="testi-card">
                        <span class="testi-quote-icon">"</span>
                        <div class="testi-stars">
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span><span class="testi-star">⭐</span>
                          <span class="testi-star">⭐</span>
                        </div>
                        <p class="testi-text">
                          "Ai Mr Sultan menyajikan persembahan terbaik berupa situs Situs Slot Gampang Menang 2026, link SITUS GACOR resmi dengan teknologi maxwin canggih terkemuka, bisa deposit 1000 dan Slot88 Resmi  deposit 1000 pertama di Indonesia."
                        </p>
                        <div class="testi-author">
                          <div class="testi-avatar">AR</div>
                          <div class="testi-author-info">
                            <span class="testi-author-name">JIN KAIRUL</span>
                            <div class="testi-author-meta">
                              <span class="testi-author-city">Makassar</span>
                              <span class="testi-author-sep"></span>
                              <span class="testi-author-time">7 hari lalu</span>
                            </div>
                          </div>
                          <div class="testi-verified">
                            <span class="testi-verified-dot"></span>
                            VERIFIED
                          </div>
                        </div>
                      </div>
              
              
              
                      <!-- Closing Testimoni -->
                      <div class="testi-closing-wrap">
                        <span class="testi-closing-icon">🏆</span>
                        <p class="testi-closing-text">
                          Jaman sekarang emang sulit buat temuin situs judi slot online di goolge, tapi Ai Mr Sultan berani jamin untuk selalu hadir bagi siapa yang mau mencari keuntungan dari game slot gacor terbaru 2026, mulai dari baca perihal slot online sampai matang, langsung depo dan jadi jutawan dalam semalam bagi kalian yang sudah cape di tipu realita kehidupan. hehe
                        </p>
                      </div>
                
                    </div><!-- end testimoni-inner -->
                  </div><!-- end rkbm-testimoni -->
                
                  <!-- ==================== CTA ==================== -->
                  <div class="rkbm-cta">
                    <div class="cta-title">Siap Bergabung dengan Ai Mr Sultan?</div>
                    <p class="cta-subtitle">
                      Daftar sekarang dan nikmati pengalaman bermain slot online terbaik
                      bersama jutaan pemain di Asia Tenggara
                    </p>
                    <div class="cta-buttons">
                      <a href="https://vanillacafes.com/matcha-latte/"
                         rel="nofollow noopener" target="_blank"
                         class="cta-btn-primary">
                        <span>🚀 DAFTAR SEKARANG</span>
                        <span>→</span>
                      </a>
                      <a href="https://vanillacafes.com/matcha-latte/"
                         rel="nofollow noopener" target="_blank"
                         class="cta-btn-secondary">
                        <span>💬 LIVE CHAT</span>
                        <span>→</span>
                      </a>
                    </div>
                  </div>
                
                </div><!-- end RKBM-wrapper -->
                
                <!-- ============================================
                     JAVASCRIPT LENGKAP
                ============================================ -->
                <script>
                (function () {
                
                  /* ============================================
                     FAQ ACCORDION
                  ============================================ */
                  var faqItems = document.querySelectorAll('.faq-item-new');
                
                  faqItems.forEach(function (item) {
                    var btn = item.querySelector('.faq-btn-new');
                    var icon = item.querySelector('.faq-toggle-icon');
                
                    btn.addEventListener('click', function () {
                      var isOpen = item.classList.contains('faq-open');
                
                      /* Tutup semua */
                      faqItems.forEach(function (other) {
                        other.classList.remove('faq-open');
                        var otherIcon = other.querySelector('.faq-toggle-icon');
                        if (otherIcon) otherIcon.textContent = '+';
                      });
                
                      /* Buka yang diklik */
                      if (!isOpen) {
                        item.classList.add('faq-open');
                        if (icon) icon.textContent = '×';
                      }
                    });
                  });
                
                  /* ============================================
                     INTERSECTION OBSERVER - ANIMASI MASUK
                  ============================================ */
                  var ioOptions = {
                    threshold: 0.12,
                    rootMargin: '0px 0px -40px 0px'
                  };
                
                  var io = new IntersectionObserver(function (entries) {
                    entries.forEach(function (entry) {
                      if (entry.isIntersecting) {
                        entry.target.classList.add('io-visible');
                        io.unobserve(entry.target);
                      }
                    });
                  }, ioOptions);
                
                  /* Inject style io-visible */
                  var ioStyle = document.createElement('style');
                  ioStyle.textContent = '.io-visible { opacity:1 !important; transform:none !important; }';
                  document.head.appendChild(ioStyle);
                
                  /* Observe content cards */
                  document.querySelectorAll('.content-card').forEach(function (el, i) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateY(35px)';
                    el.style.transition =
                      'opacity 0.6s ease ' + (i * 0.1) + 's, ' +
                      'transform 0.6s ease ' + (i * 0.1) + 's';
                    io.observe(el);
                  });
                
                  /* Observe stat items */
                  document.querySelectorAll('.stat-item').forEach(function (el, i) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateY(30px)';
                    el.style.transition =
                      'opacity 0.5s ease ' + (i * 0.1) + 's, ' +
                      'transform 0.5s ease ' + (i * 0.1) + 's';
                    io.observe(el);
                  });
                
                  /* Observe faq items */
                  document.querySelectorAll('.faq-item-new').forEach(function (el, i) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateX(-25px)';
                    el.style.transition =
                      'opacity 0.5s ease ' + (i * 0.07) + 's, ' +
                      'transform 0.5s ease ' + (i * 0.07) + 's';
                    io.observe(el);
                  });
                
                  /* Observe testi cards */
                  document.querySelectorAll('.testi-card').forEach(function (el, i) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateY(40px) scale(0.96)';
                    el.style.transition =
                      'opacity 0.6s ease ' + (i * 0.08) + 's, ' +
                      'transform 0.6s ease ' + (i * 0.08) + 's';
                    io.observe(el);
                  });
                
                  /* Observe section titles */
                  document.querySelectorAll('.section-title-wrap').forEach(function (el) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateY(25px)';
                    el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                    io.observe(el);
                  });
                
                  /* Observe closing wrap */
                  document.querySelectorAll('.testi-closing-wrap').forEach(function (el) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateY(25px)';
                    el.style.transition = 'opacity 0.6s ease 0.3s, transform 0.6s ease 0.3s';
                    io.observe(el);
                  });
                
                  /* Observe hero badge */
                  document.querySelectorAll('.rkbm-hero-badge').forEach(function (el) {
                    el.style.opacity = '0';
                    el.style.transform = 'translateY(20px)';
                    el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                    io.observe(el);
                  });
                
                  /* ============================================
                     COUNTER ANIMASI STATS
                  ============================================ */
                  function animateCount(el, endVal, suffix, duration) {
                    var startTime = null;
                
                    function step(ts) {
                      if (!startTime) startTime = ts;
                      var progress = Math.min((ts - startTime) / duration, 1);
                      var eased    = 1 - Math.pow(1 - progress, 3);
                      var current  = Math.floor(eased * endVal);
                      el.textContent = current + suffix;
                      if (progress < 1) requestAnimationFrame(step);
                    }
                    requestAnimationFrame(step);
                  }
                
                  var statsObserver = new IntersectionObserver(function (entries) {
                    entries.forEach(function (entry) {
                      if (!entry.isIntersecting) return;
                
                      var statValues = entry.target.querySelectorAll('.stat-value');
                      statValues.forEach(function (el) {
                        var raw = el.textContent.trim();
                        if (raw.includes('500K+')) animateCount(el, 500, 'K+', 1800);
                        if (raw.includes('1000+')) animateCount(el, 1000, '+', 2000);
                        if (raw.includes('99%'))   animateCount(el, 99,   '%', 1500);
                        if (raw.includes('24/7'))  { /* static */ }
                      });
                
                      statsObserver.unobserve(entry.target);
                    });
                  }, { threshold: 0.5 });
                
                  var statsEl = document.querySelector('.rkbm-stats');
                  if (statsEl) statsObserver.observe(statsEl);
                
                  /* ============================================
                     HERO SLIDE UP ON LOAD
                  ============================================ */
                  var hero = document.querySelector('.rkbm-hero');
                  if (hero) {
                    hero.style.opacity  = '0';
                    hero.style.transform = 'translateY(30px)';
                    hero.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
                    setTimeout(function () {
                      hero.style.opacity   = '1';
                      hero.style.transform = 'translateY(0)';
                    }, 200);
                  }
                
                  /* ============================================
                     TESTI CARD - TOUCH ACTIVE (MOBILE)
                  ============================================ */
                  document.querySelectorAll('.testi-card').forEach(function (card) {
                    card.addEventListener('touchstart', function () {
                      this.style.transform = 'translateY(-6px) scale(1.01)';
                    }, { passive: true });
                    card.addEventListener('touchend', function () {
                      var self = this;
                      setTimeout(function () {
                        self.style.transform = '';
                      }, 300);
                    }, { passive: true });
                  });
                
                  /* ============================================
                     SMOOTH SCROLL UNTUK CTA BUTTON
                  ============================================ */
                  document.querySelectorAll('a[href^="#"]').forEach(function (anchor) {
                    anchor.addEventListener('click', function (e) {
                      var target = document.querySelector(this.getAttribute('href'));
                      if (target) {
                        e.preventDefault();
                        target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                      }
                    });
                  });
                
                  /* ============================================
                     CHIP HOVER RIPPLE EFFECT
                  ============================================ */
                  document.querySelectorAll('.hero-chip').forEach(function (chip) {
                    chip.addEventListener('mouseenter', function () {
                      this.style.transition = 'all 0.3s cubic-bezier(0.34,1.56,0.64,1)';
                    });
                  });
                
                  /* ============================================
                     FAQ KEYBOARD ACCESSIBILITY
                  ============================================ */
                  document.querySelectorAll('.faq-btn-new').forEach(function (btn) {
                    btn.setAttribute('aria-expanded', 'false');
                    btn.addEventListener('keydown', function (e) {
                      if (e.key === 'Enter' || e.key === ' ') {
                        e.preventDefault();
                        btn.click();
                        var expanded = btn.closest('.faq-item-new').classList.contains('faq-open');
                        btn.setAttribute('aria-expanded', expanded ? 'true' : 'false');
                      }
                    });
                  });
                
                })();
                </script>


Tempus quam pellentesque nec nam aliquam sem. Risus at ultrices mi tempus imperdiet. Id porta nibh venenatis cras sed felis eget velit. Ipsum a arcu cursus vitae. Facilisis magna etiam tempor orci eu lobortis elementum. Tincidunt dui ut ornare lectus sit. Quisque non tellus orci ac. Blandit libero volutpat sed cras. Nec tincidunt praesent semper feugiat nibh sed pulvinar proin gravida. Egestas integer eget aliquet nibh praesent tristique magna.
