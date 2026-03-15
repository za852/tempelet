<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Canva Designer Power Bundle</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800;900&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --primary: #7C3AED;
  --primary-dark: #5B21B6;
  --accent: #F59E0B;
  --accent-dark: #D97706;
  --danger: #EF4444;
  --success: #10B981;
  --whatsapp: #25D366;
  --whatsapp-dark: #128C7E;
  --dark: #1F2937;
  --light: #F9FAFB;
  --gray: #6B7280;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Tajawal', sans-serif;
  background: #0F0F1A;
  color: #E5E7EB;
  overflow-x: hidden;
  line-height: 1.7;
  width: 100%;
  min-height: 100vh;
}

.container {
  max-width: 900px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Top Bar */
.top-bar {
  background: linear-gradient(90deg, var(--danger), #DC2626);
  padding: 10px 0;
  text-align: center;
  font-weight: 700;
  font-size: 14px;
  color: white;
  animation: pulse-bg 2s infinite;
  position: sticky;
  top: 0;
  z-index: 1000;
}

@keyframes pulse-bg {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.85; }
}

.top-bar span {
  animation: blink 1s infinite;
}

@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

/* Hero Section */
.hero {
  background: linear-gradient(135deg, #1a1035 0%, #0F0F1A 50%, #1a0a2e 100%);
  padding: 60px 0 50px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.hero::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle at 30% 50%, rgba(124,58,237,0.1) 0%, transparent 50%),
              radial-gradient(circle at 70% 50%, rgba(245,158,11,0.08) 0%, transparent 50%);
  animation: rotate-bg 20s linear infinite;
}

@keyframes rotate-bg {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.hero .container {
  position: relative;
  z-index: 1;
}

.badge {
  display: inline-block;
  background: linear-gradient(135deg, var(--accent), var(--accent-dark));
  color: #000;
  padding: 6px 24px;
  border-radius: 50px;
  font-weight: 800;
  font-size: 15px;
  margin-bottom: 24px;
}

.hero h1 {
  font-size: clamp(26px, 5vw, 42px);
  font-weight: 900;
  color: white;
  line-height: 1.4;
  margin-bottom: 20px;
  max-width: 750px;
  margin-left: auto;
  margin-right: auto;
}

.hero h1 span {
  background: linear-gradient(135deg, var(--accent), #FBBF24);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-sub {
  font-size: clamp(16px, 2.5vw, 20px);
  color: #9CA3AF;
  margin-bottom: 30px;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.price-hero {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
  margin-bottom: 10px;
  flex-wrap: wrap;
}

.old-price {
  font-size: clamp(24px, 4vw, 36px);
  color: var(--danger);
  text-decoration: line-through;
  font-weight: 700;
  opacity: 0.7;
}

.new-price {
  font-size: clamp(42px, 7vw, 64px);
  font-weight: 900;
  color: var(--success);
  text-shadow: 0 0 30px rgba(16,185,129,0.3);
}

.discount-badge {
  background: var(--danger);
  color: white;
  padding: 8px 20px;
  border-radius: 12px;
  font-weight: 800;
  font-size: 22px;
  display: inline-block;
  margin-bottom: 25px;
  animation: shake 2s infinite;
  box-shadow: 0 4px 20px rgba(239,68,68,0.4);
}

@keyframes shake {
  0%, 100% { transform: rotate(0deg); }
  5% { transform: rotate(-3deg); }
  10% { transform: rotate(3deg); }
  15% { transform: rotate(0deg); }
}

/* WhatsApp CTA Button */
.cta-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  background: linear-gradient(135deg, var(--whatsapp), var(--whatsapp-dark));
  color: white;
  padding: 18px 50px;
  border-radius: 16px;
  font-size: clamp(18px, 3vw, 24px);
  font-weight: 900;
  text-decoration: none;
  border: none;
  cursor: pointer;
  transition: all 0.3s;
  box-shadow: 0 8px 30px rgba(37,211,102,0.35);
  font-family: 'Tajawal', sans-serif;
  position: relative;
  overflow: hidden;
}

.cta-btn::after {
  content: '';
  position: absolute;
  top: -50%;
  left: -100%;
  width: 60%;
  height: 200%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.25), transparent);
  transform: skewX(-15deg);
  animation: shimmer 2.5s infinite;
}

@keyframes shimmer {
  0% { left: -100%; }
  100% { left: 200%; }
}

.cta-btn:hover {
  transform: translateY(-3px) scale(1.03);
  box-shadow: 0 12px 40px rgba(37,211,102,0.5);
}

.cta-btn .wa-icon {
  font-size: 28px;
  line-height: 1;
}

.cta-btn-gold {
  background: linear-gradient(135deg, var(--accent), #F97316);
  color: #000;
  box-shadow: 0 8px 30px rgba(245,158,11,0.4);
}

.cta-btn-gold:hover {
  box-shadow: 0 12px 40px rgba(245,158,11,0.5);
}

.cta-sub {
  margin-top: 12px;
  font-size: 14px;
  color: #9CA3AF;
}

.cta-sub span {
  color: var(--success);
  font-weight: 700;
}

/* Timer */
.timer-section {
  background: rgba(239,68,68,0.1);
  border: 1px solid rgba(239,68,68,0.3);
  border-radius: 16px;
  padding: 20px;
  margin-top: 30px;
  max-width: 500px;
  margin-left: auto;
  margin-right: auto;
}

.timer-title {
  color: var(--danger);
  font-weight: 800;
  font-size: 16px;
  margin-bottom: 12px;
}

.timer-boxes {
  display: flex;
  justify-content: center;
  gap: 12px;
  direction: ltr;
}

.timer-box {
  background: rgba(239,68,68,0.15);
  border: 1px solid rgba(239,68,68,0.3);
  border-radius: 12px;
  padding: 12px 16px;
  min-width: 65px;
  text-align: center;
}

.timer-box .num {
  font-size: 28px;
  font-weight: 900;
  color: white;
  display: block;
  font-variant-numeric: tabular-nums;
}

.timer-box .lbl {
  font-size: 11px;
  color: #9CA3AF;
  margin-top: 2px;
}

/* Sections */
section {
  padding: 50px 0;
}

.section-title {
  font-size: clamp(22px, 4vw, 34px);
  font-weight: 900;
  text-align: center;
  margin-bottom: 16px;
  color: white;
}

.section-title span {
  background: linear-gradient(135deg, var(--primary), #A78BFA);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.section-sub {
  text-align: center;
  color: #9CA3AF;
  font-size: 17px;
  margin-bottom: 40px;
  max-width: 650px;
  margin-left: auto;
  margin-right: auto;
}

/* Product Display */
.product-display {
  background: linear-gradient(135deg, #1a1035, #150d28);
}

.product-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  margin-bottom: 30px;
}

.product-card {
  background: rgba(124,58,237,0.1);
  border: 1px solid rgba(124,58,237,0.25);
  border-radius: 20px;
  padding: 30px;
  text-align: center;
  transition: transform 0.3s;
}

.product-card:hover {
  transform: translateY(-5px);
}

.product-icon {
  font-size: 64px;
  margin-bottom: 16px;
  display: block;
}

.product-card h3 {
  font-size: 20px;
  font-weight: 800;
  color: white;
  margin-bottom: 10px;
}

.product-card p {
  color: #9CA3AF;
  font-size: 15px;
}

.bundle-tag {
  background: linear-gradient(135deg, var(--primary), var(--accent));
  text-align: center;
  padding: 16px;
  border-radius: 14px;
  font-weight: 800;
  font-size: 20px;
  color: white;
  max-width: 500px;
  margin: 0 auto;
}

/* Problem Section */
.problem-section {
  background: linear-gradient(135deg, #1a0505, #0F0F1A);
}

.problem-list {
  max-width: 650px;
  margin: 0 auto;
}

.problem-item {
  display: flex;
  align-items: flex-start;
  gap: 16px;
  padding: 16px 0;
  border-bottom: 1px solid rgba(255,255,255,0.05);
}

.problem-item .icon {
  font-size: 28px;
  flex-shrink: 0;
}

.problem-item p {
  font-size: 17px;
  color: #D1D5DB;
}

/* Solution */
.solution-section {
  background: linear-gradient(135deg, #051a0f, #0F0F1A);
}

.solution-box {
  background: rgba(16,185,129,0.08);
  border: 1px solid rgba(16,185,129,0.25);
  border-radius: 20px;
  padding: 40px;
  text-align: center;
  max-width: 700px;
  margin: 0 auto;
}

.solution-box .big-icon {
  font-size: 64px;
  margin-bottom: 20px;
}

.solution-box h3 {
  font-size: 24px;
  font-weight: 800;
  color: var(--success);
  margin-bottom: 16px;
}

.solution-box p {
  font-size: 17px;
  color: #D1D5DB;
  line-height: 1.8;
}

/* What You Get */
.get-section {
  background: #0F0F1A;
}

.get-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 16px;
  max-width: 700px;
  margin: 0 auto;
}

.get-item {
  display: flex;
  align-items: center;
  gap: 14px;
  background: rgba(124,58,237,0.08);
  border: 1px solid rgba(124,58,237,0.15);
  border-radius: 14px;
  padding: 18px 20px;
  transition: all 0.3s;
}

.get-item:hover {
  background: rgba(124,58,237,0.15);
  transform: translateX(-5px);
}

.get-item .icon {
  font-size: 28px;
  flex-shrink: 0;
}

.get-item span {
  font-size: 16px;
  font-weight: 600;
  color: white;
}

/* Features */
.features-section {
  background: linear-gradient(135deg, #1a1035, #0F0F1A);
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 20px;
}

.feature-card {
  background: rgba(255,255,255,0.03);
  border: 1px solid rgba(255,255,255,0.08);
  border-radius: 16px;
  padding: 28px;
  text-align: center;
  transition: all 0.3s;
}

.feature-card:hover {
  background: rgba(124,58,237,0.1);
  border-color: rgba(124,58,237,0.3);
  transform: translateY(-3px);
}

.feature-card .icon {
  font-size: 40px;
  margin-bottom: 14px;
}

.feature-card h4 {
  font-size: 17px;
  font-weight: 800;
  color: white;
  margin-bottom: 8px;
}

.feature-card p {
  color: #9CA3AF;
  font-size: 14px;
}

/* Value Comparison */
.value-section {
  background: #0F0F1A;
}

.value-table {
  max-width: 600px;
  margin: 0 auto;
  background: rgba(255,255,255,0.03);
  border-radius: 20px;
  overflow: hidden;
  border: 1px solid rgba(255,255,255,0.08);
}

.value-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 18px 24px;
  border-bottom: 1px solid rgba(255,255,255,0.05);
}

.value-row:last-child {
  border-bottom: none;
}

.value-row .name {
  font-size: 16px;
  color: #D1D5DB;
}

.value-row .price {
  font-size: 16px;
  font-weight: 700;
  color: #9CA3AF;
}

.value-total {
  background: rgba(239,68,68,0.1);
  padding: 18px 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.value-total .name {
  font-weight: 800;
  color: white;
  font-size: 18px;
}

.value-total .price {
  font-weight: 800;
  color: var(--danger);
  font-size: 20px;
  text-decoration: line-through;
}

.value-deal {
  background: linear-gradient(135deg, rgba(16,185,129,0.15), rgba(16,185,129,0.05));
  border: 2px solid var(--success);
  padding: 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.value-deal .name {
  font-weight: 900;
  color: var(--success);
  font-size: 20px;
}

.value-deal .price {
  font-weight: 900;
  color: var(--success);
  font-size: 28px;
}

/* Reviews */
.reviews-section {
  background: linear-gradient(135deg, #1a1035, #0F0F1A);
}

.reviews-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
  gap: 20px;
}

.review-card {
  background: rgba(255,255,255,0.04);
  border: 1px solid rgba(255,255,255,0.08);
  border-radius: 16px;
  padding: 24px;
}

.review-stars {
  color: var(--accent);
  font-size: 20px;
  margin-bottom: 12px;
}

.review-text {
  font-size: 15px;
  color: #D1D5DB;
  margin-bottom: 16px;
  line-height: 1.7;
  font-style: italic;
}

.review-author {
  display: flex;
  align-items: center;
  gap: 12px;
}

.review-avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--primary), var(--accent));
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 20px;
}

.review-name {
  font-weight: 700;
  color: white;
  font-size: 14px;
}

.review-role {
  font-size: 12px;
  color: #9CA3AF;
}

/* FOMO */
.fomo-section {
  background: linear-gradient(135deg, #1a0505, #0F0F1A);
  text-align: center;
}

.fomo-box {
  background: rgba(239,68,68,0.08);
  border: 2px solid rgba(239,68,68,0.3);
  border-radius: 20px;
  padding: 40px;
  max-width: 650px;
  margin: 0 auto;
}

.fomo-box .big-icon {
  font-size: 56px;
  margin-bottom: 16px;
}

.fomo-box h3 {
  font-size: 24px;
  font-weight: 900;
  color: var(--danger);
  margin-bottom: 16px;
}

.fomo-box p {
  font-size: 17px;
  color: #D1D5DB;
  line-height: 1.8;
}

.fomo-highlight {
  color: var(--accent) !important;
  font-weight: 800;
}

/* Target Audience */
.audience-section {
  background: #0F0F1A;
}

.audience-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
  max-width: 700px;
  margin: 0 auto;
}

.audience-item {
  background: rgba(124,58,237,0.08);
  border: 1px solid rgba(124,58,237,0.2);
  border-radius: 14px;
  padding: 24px;
  text-align: center;
  transition: all 0.3s;
}

.audience-item:hover {
  background: rgba(124,58,237,0.15);
  transform: scale(1.03);
}

.audience-item .icon {
  font-size: 36px;
  margin-bottom: 10px;
}

.audience-item span {
  font-weight: 700;
  color: white;
  font-size: 15px;
}

/* Final CTA */
.final-cta {
  background: linear-gradient(135deg, #1a1035, #251545);
  text-align: center;
  padding: 60px 0;
}

.final-cta .container {
  max-width: 650px;
}

.final-price-box {
  background: rgba(16,185,129,0.08);
  border: 2px solid rgba(16,185,129,0.3);
  border-radius: 20px;
  padding: 30px;
  margin: 30px 0;
}

/* Trust */
.trust-section {
  background: #0F0F1A;
  padding-bottom: 60px;
}

.trust-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  max-width: 700px;
  margin: 0 auto;
}

.trust-item {
  text-align: center;
  padding: 24px;
}

.trust-item .icon {
  font-size: 40px;
  margin-bottom: 12px;
}

.trust-item h4 {
  font-weight: 800;
  color: white;
  margin-bottom: 6px;
  font-size: 16px;
}

.trust-item p {
  color: #9CA3AF;
  font-size: 14px;
}

/* Footer */
footer {
  background: rgba(0,0,0,0.3);
  text-align: center;
  padding: 24px;
  color: #6B7280;
  font-size: 13px;
}

/* Floating WhatsApp Button */
.wa-floating {
  position: fixed;
  bottom: 90px;
  left: 20px;
  z-index: 1001;
  display: flex;
  align-items: center;
  gap: 0;
  animation: float-wa 3s ease-in-out infinite;
}

.wa-floating-btn {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  background: linear-gradient(135deg, #25D366, #128C7E);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 34px;
  text-decoration: none;
  box-shadow: 0 6px 24px rgba(37,211,102,0.5);
  transition: all 0.3s;
  position: relative;
  cursor: pointer;
}

.wa-floating-btn:hover {
  transform: scale(1.12);
  box-shadow: 0 8px 32px rgba(37,211,102,0.6);
}

.wa-floating-btn .wa-ping {
  position: absolute;
  top: -2px;
  right: -2px;
  width: 18px;
  height: 18px;
  background: var(--danger);
  border-radius: 50%;
  border: 2px solid #0F0F1A;
  animation: pulse-dot 1.5s infinite;
}

.wa-tooltip {
  background: rgba(15,15,26,0.95);
  border: 1px solid rgba(37,211,102,0.4);
  border-radius: 12px;
  padding: 10px 16px;
  margin-right: 12px;
  color: white;
  font-size: 13px;
  font-weight: 700;
  white-space: nowrap;
  backdrop-filter: blur(10px);
  opacity: 0;
  transform: translateX(-10px);
  transition: all 0.3s;
  pointer-events: none;
}

.wa-floating:hover .wa-tooltip {
  opacity: 1;
  transform: translateX(0);
}

@keyframes float-wa {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-8px); }
}

/* Social proof bar */
.social-proof-bar {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: rgba(15,15,26,0.95);
  border: 1px solid rgba(124,58,237,0.3);
  border-radius: 12px;
  padding: 12px 20px;
  display: flex;
  align-items: center;
  gap: 10px;
  z-index: 999;
  animation: slide-up 0.5s ease;
  backdrop-filter: blur(10px);
  font-size: 13px;
}

@keyframes slide-up {
  from { transform: translateY(100px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

.live-dot {
  width: 8px;
  height: 8px;
  background: var(--success);
  border-radius: 50%;
  animation: pulse-dot 1.5s infinite;
}

@keyframes pulse-dot {
  0%, 100% { box-shadow: 0 0 0 0 rgba(16,185,129,0.5); }
  50% { box-shadow: 0 0 0 6px rgba(16,185,129,0); }
}

/* Floating CTA on mobile */
.floating-cta {
  display: none;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(15,15,26,0.97);
  border-top: 1px solid rgba(37,211,102,0.4);
  padding: 10px 16px;
  z-index: 998;
  backdrop-filter: blur(10px);
}

.floating-cta a.cta-btn {
  width: 100%;
  text-align: center;
  padding: 14px 20px;
  font-size: 17px;
}

/* WhatsApp animated banner */
.wa-banner {
  background: linear-gradient(135deg, rgba(37,211,102,0.12), rgba(18,140,126,0.08));
  border: 2px solid rgba(37,211,102,0.35);
  border-radius: 20px;
  padding: 30px;
  text-align: center;
  max-width: 600px;
  margin: 30px auto 0;
  position: relative;
  overflow: hidden;
}

.wa-banner::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background: linear-gradient(45deg, transparent 30%, rgba(37,211,102,0.05) 50%, transparent 70%);
  animation: wa-sweep 3s infinite;
}

@keyframes wa-sweep {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}

.wa-banner-content {
  position: relative;
  z-index: 1;
}

.wa-banner h3 {
  font-size: 20px;
  font-weight: 900;
  color: var(--whatsapp);
  margin-bottom: 10px;
}

.wa-banner p {
  color: #D1D5DB;
  font-size: 15px;
  margin-bottom: 16px;
}

.wa-steps {
  display: flex;
  justify-content: center;
  gap: 24px;
  flex-wrap: wrap;
  margin-bottom: 20px;
}

.wa-step {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 6px;
}

.wa-step .step-num {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  background: var(--whatsapp);
  color: white;
  font-weight: 900;
  font-size: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.wa-step .step-text {
  font-size: 13px;
  color: #9CA3AF;
  font-weight: 600;
}

/* Sold counter */
.sold-counter {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  background: rgba(245,158,11,0.1);
  border: 1px solid rgba(245,158,11,0.3);
  padding: 8px 20px;
  border-radius: 50px;
  margin-top: 16px;
  font-size: 14px;
  color: var(--accent);
  font-weight: 600;
}

@media (max-width: 768px) {
  .floating-cta {
    display: block;
  }
  
  .social-proof-bar {
    bottom: 64px;
    right: 10px;
    left: 10px;
    justify-content: center;
    font-size: 12px;
    padding: 8px 12px;
  }
  
  .wa-floating {
    bottom: 75px;
    left: 12px;
  }

  .wa-floating-btn {
    width: 54px;
    height: 54px;
    font-size: 28px;
  }
  
  section {
    padding: 40px 0;
  }
  
  .hero {
    padding: 40px 0 40px;
  }
  
  .solution-box, .fomo-box {
    padding: 24px;
  }

  .wa-banner {
    padding: 20px;
  }
}

/* Animations on scroll */
.animate-in {
  opacity: 0;
  transform: translateY(30px);
  transition: all 0.6s ease;
}

.animate-in.visible {
  opacity: 1;
  transform: translateY(0);
}
</style>
</head>
<body>

<!-- Top Urgency Bar -->
<div class="top-bar">
  <span>🔥</span> العرض ينتهي قريبًا – خصم 70% لفترة محدودة جدًا! <span>🔥</span>
</div>

<!-- Hero Section -->
<section class="hero">
  <div class="container">
    <div class="badge">🎨 عرض حصري لفترة محدودة</div>
    <h1>أنشئ عروضًا احترافية لتصاميمك في Canva خلال ثوانٍ – <span>بدون خبرة تصميم</span></h1>
    <p class="hero-sub">احصل على حزمة Mockup الكاملة + أكثر من 110 Digital Paper جاهزة للاستخدام مباشرة داخل Canva</p>
    
    <div class="discount-badge">🔥 خصم 70% اليوم فقط!</div>
    
    <div class="price-hero">
      <span class="old-price">\$4.50</span>
      <span class="new-price">\$1.35</span>
    </div>
    
    <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="cta-btn">
      <span class="wa-icon">💬</span>
      اطلب عبر واتساب الآن
    </a>
    <div class="cta-sub">⚡ <span>رد فوري</span> على واتساب | 🔒 شراء آمن 100%</div>
    
    <div class="sold-counter">
      <span>🔥</span> <span id="sold-count">847</span> شخص اشتروا هذه الحزمة
    </div>
    
    <div class="timer-section">
      <div class="timer-title">⏰ العرض ينتهي خلال:</div>
      <div class="timer-boxes">
        <div class="timer-box">
          <span class="num" id="hours">02</span>
          <span class="lbl">ساعة</span>
        </div>
        <div class="timer-box">
          <span class="num" id="minutes">47</span>
          <span class="lbl">دقيقة</span>
        </div>
        <div class="timer-box">
          <span class="num" id="seconds">33</span>
          <span class="lbl">ثانية</span>
        </div>
      </div>
    </div>

    <!-- WhatsApp Steps Banner -->
    <div class="wa-banner animate-in">
      <div class="wa-banner-content">
        <h3>💬 كيف تشتري عبر واتساب؟</h3>
        <div class="wa-steps">
          <div class="wa-step">
            <span class="step-num">1</span>
            <span class="step-text">اضغط الزر</span>
          </div>
          <div class="wa-step">
            <span class="step-num">2</span>
            <span class="step-text">أرسل الرسالة</span>
          </div>
          <div class="wa-step">
            <span class="step-num">3</span>
            <span class="step-text">استلم الحزمة فورًا</span>
          </div>
        </div>
        <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="cta-btn" style="font-size:17px; padding:14px 36px;">
          <span class="wa-icon">💬</span>
          ابدأ المحادثة الآن
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Product Display -->
<section class="product-display">
  <div class="container">
    <h2 class="section-title animate-in">ماذا يوجد داخل <span>الحزمة؟</span></h2>
    <p class="section-sub animate-in">حزمتان احترافيتان في عرض واحد لا يُصدق 🤯</p>
    
    <div class="product-cards">
      <div class="product-card animate-in">
        <span class="product-icon">🎨</span>
        <h3>Ultimate Canva Mockup Bundle</h3>
        <p>مجموعة شاملة من قوالب الموك أب الاحترافية المصممة خصيصًا لـ Canva – اعرض تصاميمك بشكل مذهل</p>
      </div>
      <div class="product-card animate-in">
        <span class="product-icon">📄</span>
        <h3>110+ Digital Paper Mockup</h3>
        <p>أكثر من 110 خلفية ورقية رقمية عالية الجودة – مثالية لعرض منتجاتك الرقمية بأناقة</p>
      </div>
    </div>
    
    <div class="bundle-tag animate-in">🎁 حزمتان كاملتان بسعر واحد = \$1.35 فقط!</div>
  </div>
</section>

<!-- Problem Section -->
<section class="problem-section">
  <div class="container">
    <h2 class="section-title animate-in">😩 هل تعاني من هذه <span>المشاكل؟</span></h2>
    
    <div class="problem-list">
      <div class="problem-item animate-in">
        <span class="icon">😤</span>
        <p>تقضي ساعات طويلة في محاولة إنشاء موك أب احترافي لمنتجاتك الرقمية</p>
      </div>
      <div class="problem-item animate-in">
        <span class="icon">😞</span>
        <p>تبحث في كل مكان عن خلفيات رقمية عالية الجودة لكن لا تجد ما يناسبك</p>
      </div>
      <div class="problem-item animate-in">
        <span class="icon">💸</span>
        <p>تدفع مبالغ كبيرة على أدوات تصميم معقدة مثل فوتوشوب دون أن تستخدمها بالكامل</p>
      </div>
      <div class="problem-item animate-in">
        <span class="icon">😰</span>
        <p>تصاميمك لا تبدو احترافية عند عرضها مما يؤثر على مبيعاتك ومصداقيتك</p>
      </div>
      <div class="problem-item animate-in">
        <span class="icon">⏰</span>
        <p>ليس لديك الوقت لتعلم أدوات التصميم المعقدة وتحتاج حلاً سريعًا وفعالًا</p>
      </div>
    </div>
  </div>
</section>

<!-- Solution Section -->
<section class="solution-section">
  <div class="container">
    <h2 class="section-title animate-in">✅ إليك <span>الحل الأمثل</span></h2>
    
    <div class="solution-box animate-in">
      <div class="big-icon">🚀</div>
      <h3>Canva Designer Power Bundle</h3>
      <p>حزمة متكاملة تمنحك كل ما تحتاجه لعرض تصاميمك ومنتجاتك الرقمية بشكل احترافي مذهل – مباشرة داخل Canva، بدون أي خبرة تصميم سابقة، وبدون الحاجة لأي برنامج آخر. فقط افتح Canva، اختر القالب، عدّل، وانشر!</p>
    </div>
    
    <div style="text-align:center; margin-top: 30px;">
      <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="cta-btn">
        <span class="wa-icon">💬</span>
        اطلب عبر واتساب – \$1.35 فقط
      </a>
    </div>
  </div>
</section>

<!-- What You Get -->
<section class="get-section">
  <div class="container">
    <h2 class="section-title animate-in">📦 ماذا ستحصل عليه <span>بالتفصيل</span></h2>
    <p class="section-sub animate-in">كل هذا مقابل أقل من سعر كوب قهوة! ☕</p>
    
    <div class="get-grid">
      <div class="get-item animate-in">
        <span class="icon">🎨</span>
        <span>Ultimate Canva Mockup Bundle</span>
      </div>
      <div class="get-item animate-in">
        <span class="icon">📄</span>
        <span>أكثر من 110 Digital Paper</span>
      </div>
      <div class="get-item animate-in">
        <span class="icon">🖼️</span>
        <span>قوالب Mockup احترافية</span>
      </div>
      <div class="get-item animate-in">
        <span class="icon">✏️</span>
        <span>ملفات سهلة التعديل</span>
      </div>
      <div class="get-item animate-in">
        <span class="icon">⚡</span>
        <span>استخدام مباشر داخل Canva</span>
      </div>
      <div class="get-item animate-in">
        <span class="icon">♾️</span>
        <span>وصول دائم للملفات</span>
      </div>
    </div>
  </div>
</section>

<!-- Features -->
<section class="features-section">
  <div class="container">
    <h2 class="section-title animate-in">⭐ مميزات <span>الحزمة</span></h2>
    
    <div class="features-grid">
      <div class="feature-card animate-in">
        <div class="icon">🎯</div>
        <h4>تعمل بالكامل داخل Canva</h4>
        <p>لا حاجة لأي برنامج خارجي</p>
      </div>
      <div class="feature-card animate-in">
        <div class="icon">🚫</div>
        <h4>لا تحتاج فوتوشوب</h4>
        <p>وفّر اشتراكك الشهري</p>
      </div>
      <div class="feature-card animate-in">
        <div class="icon">👆</div>
        <h4>سهلة الاستخدام</h4>
        <p>فقط اسحب وأفلت تصميمك</p>
      </div>
      <div class="feature-card animate-in">
        <div class="icon">💎</div>
        <h4>جودة عالية جدًا</h4>
        <p>دقة احترافية لكل الاستخدامات</p>
      </div>
      <div class="feature-card animate-in">
        <div class="icon">🛍️</div>
        <h4>مناسبة لعرض المنتجات</h4>
        <p>مثالية لمتاجر Etsy و Gumroad</p>
      </div>
      <div class="feature-card animate-in">
        <div class="icon">⏱️</div>
        <h4>توفير الوقت</h4>
        <p>إنجاز العمل في ثوانٍ معدودة</p>
      </div>
    </div>
  </div>
</section>

<!-- Value Comparison -->
<section class="value-section">
  <div class="container">
    <h2 class="section-title animate-in">💰 قارن <span>القيمة بنفسك</span></h2>
    <p class="section-sub animate-in">لو اشتريت هذه الموارد بشكل منفصل ستدفع أكثر من 30 دولار!</p>
    
    <div class="value-table animate-in">
      <div class="value-row">
        <span class="name">🎨 حزمة Mockup احترافية</span>
        <span class="price">\$15+</span>
      </div>
      <div class="value-row">
        <span class="name">📄 110+ Digital Paper</span>
        <span class="price">\$12+</span>
      </div>
      <div class="value-row">
        <span class="name">⏰ ساعات البحث والتصميم</span>
        <span class="price">\$5+</span>
      </div>
      <div class="value-total">
        <span class="name">القيمة الإجمالية</span>
        <span class="price">\$32+</span>
      </div>
      <div class="value-deal">
        <span class="name">✨ سعرك اليوم</span>
        <span class="price">\$1.35</span>
      </div>
    </div>
    
    <div style="text-align:center; margin-top: 30px;">
      <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="cta-btn">
        <span class="wa-icon">💬</span>
        نعم! أريد هذه الصفقة عبر واتساب
      </a>
    </div>
  </div>
</section>

<!-- Reviews -->
<section class="reviews-section">
  <div class="container">
    <h2 class="section-title animate-in">💬 ماذا يقول <span>عملاؤنا؟</span></h2>
    <p class="section-sub animate-in">أكثر من 847 مصمم ومسوق يستخدمون هذه الحزمة</p>
    
    <div class="reviews-grid">
      <div class="review-card animate-in">
        <div class="review-stars">⭐⭐⭐⭐⭐</div>
        <p class="review-text">"هذه الحزمة غيّرت طريقة عرض منتجاتي بالكامل! أصبحت تصاميمي تبدو احترافية جدًا وزادت مبيعاتي على Etsy بشكل ملحوظ."</p>
        <div class="review-author">
          <div class="review-avatar">👩</div>
          <div>
            <div class="review-name">سارة أحمد</div>
            <div class="review-role">بائعة على Etsy</div>
          </div>
        </div>
      </div>
      
      <div class="review-card animate-in">
        <div class="review-stars">⭐⭐⭐⭐⭐</div>
        <p class="review-text">"لا أصدق أنني حصلت على كل هذا بهذا السعر! القوالب سهلة الاستخدام وتوفر عليّ ساعات من العمل كل أسبوع."</p>
        <div class="review-author">
          <div class="review-avatar">👨</div>
          <div>
            <div class="review-name">محمد خالد</div>
            <div class="review-role">صانع محتوى رقمي</div>
          </div>
        </div>
      </div>
      
      <div class="review-card animate-in">
        <div class="review-stars">⭐⭐⭐⭐⭐</div>
        <p class="review-text">"أفضل استثمار لمتجري الرقمي! الـ Mockups احترافية جدًا وتعمل بسلاسة داخل Canva. أنصح بها بشدة."</p>
        <div class="review-author">
          <div class="review-avatar">👩</div>
          <div>
            <div class="review-name">نورة العلي</div>
            <div class="review-role">صاحبة متجر رقمي</div>
          </div>
        </div>
      </div>
      
      <div class="review-card animate-in">
        <div class="review-stars">⭐⭐⭐⭐⭐</div>
        <p class="review-text">"كنت أدفع لمصمم كل مرة لعمل Mockup. الآن أعملها بنفسي في دقائق! شكرًا لكم على هذه الحزمة الرائعة."</p>
        <div class="review-author">
          <div class="review-avatar">👨</div>
          <div>
            <div class="review-name">يوسف مراد</div>
            <div class="review-role">مسوق رقمي</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- FOMO Section -->
<section class="fomo-section">
  <div class="container">
    <div class="fomo-box animate-in">
      <div class="big-icon">⚠️</div>
      <h3>⏰ تحذير: هذا العرض لن يستمر طويلاً!</h3>
      <p>السعر الحالي <span class="fomo-highlight">\$1.35</span> هو سعر تعريفي لفترة محدودة جدًا. قريبًا سيعود السعر إلى <strong style="color:var(--danger)">\$4.50</strong> أو أكثر. لا نستطيع ضمان بقاء هذا السعر بعد انتهاء العداد التنازلي.</p>
      <br>
      <p>🔥 <strong>كل دقيقة تمر = فرصة أقل للحصول على هذا السعر</strong></p>
      <div style="margin-top: 24px;">
        <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D9%82%D8%A8%D9%84%20%D8%A7%D9%86%D8%AA%D9%87%D8%A7%D8%A1%20%D8%A7%D9%84%D8%B9%D8%B1%D8%B6%20%F0%9F%94%A5" target="_blank" class="cta-btn">
          <span class="wa-icon">💬</span>
          أريد الحزمة قبل انتهاء العرض!
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Target Audience -->
<section class="audience-section">
  <div class="container">
    <h2 class="section-title animate-in">🎯 لمن هذه <span>الحزمة؟</span></h2>
    <p class="section-sub animate-in">إذا كنت واحدًا من هؤلاء، فهذه الحزمة صُنعت من أجلك!</p>
    
    <div class="audience-grid">
      <div class="audience-item animate-in">
        <div class="icon">🎨</div>
        <span>مصممو Canva</span>
      </div>
      <div class="audience-item animate-in">
        <div class="icon">🛍️</div>
        <span>أصحاب المتاجر الرقمية</span>
      </div>
      <div class="audience-item animate-in">
        <div class="icon">📱</div>
        <span>صناع المحتوى</span>
      </div>
      <div class="audience-item animate-in">
        <div class="icon">📣</div>
        <span>المسوقون الرقميون</span>
      </div>
      <div class="audience-item animate-in">
        <div class="icon">🏪</div>
        <span>بائعو Etsy</span>
      </div>
      <div class="audience-item animate-in">
        <div class="icon">💻</div>
        <span>بائعو Gumroad</span>
      </div>
    </div>
  </div>
</section>

<!-- Final CTA -->
<section class="final-cta" id="buy-section">
  <div class="container">
    <h2 class="section-title animate-in">🚀 جاهز لتحويل <span>تصاميمك؟</span></h2>
    <p class="section-sub animate-in">لا تفوّت هذه الفرصة – راسلنا على واتساب واحصل على الحزمة فورًا!</p>
    
    <div class="final-price-box animate-in">
      <p style="font-size:16px; color:#9CA3AF; margin-bottom:8px;">Canva Designer Power Bundle</p>
      <p style="margin-bottom:4px;">
        <span style="font-size:28px; text-decoration:line-through; color:var(--danger); font-weight:700;">\$4.50</span>
      </p>
      <p style="margin-bottom:4px;">
        <span style="font-size:56px; font-weight:900; color:var(--success);">\$1.35</span>
      </p>
      <p style="margin-bottom:20px;">
        <span style="background:var(--danger); color:white; padding:4px 16px; border-radius:8px; font-weight:800; font-size:18px;">وفّر 70%</span>
      </p>
      <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="cta-btn" style="width:100%; max-width:500px;">
        <span class="wa-icon">💬</span>
        احصل على الحزمة عبر واتساب – \$1.35 فقط
      </a>
      <div class="cta-sub">⚡ <span>رد فوري</span> | 💬 شراء مباشر عبر واتساب | ♾️ وصول دائم</div>
    </div>
  </div>
</section>

<!-- Trust Section -->
<section class="trust-section">
  <div class="container">
    <h2 class="section-title animate-in">🔒 ضمان <span>الثقة</span></h2>
    
    <div class="trust-grid">
      <div class="trust-item animate-in">
        <div class="icon">⚡</div>
        <h4>تحميل فوري</h4>
        <p>احصل على ملفاتك مباشرة بعد الشراء</p>
      </div>
      <div class="trust-item animate-in">
        <div class="icon">💎</div>
        <h4>جودة عالية</h4>
        <p>ملفات احترافية بأعلى دقة ممكنة</p>
      </div>
      <div class="trust-item animate-in">
        <div class="icon">🔓</div>
        <h4>وصول مباشر</h4>
        <p>ادخل واستخدم الملفات فورًا في Canva</p>
      </div>
    </div>
  </div>
</section>

<footer>
  <p>© 2026 Canva Designer Power Bundle – جميع الحقوق محفوظة</p>
  <p style="margin-top:8px; font-size:12px;">💬 للتواصل والشراء عبر واتساب: <a href="https://wa.me/9647515538709" target="_blank" style="color:var(--whatsapp); text-decoration:none; font-weight:700;">اضغط هنا</a></p>
</footer>

<!-- Floating WhatsApp Button -->
<div class="wa-floating" id="waFloating">
  <span class="wa-tooltip">💬 راسلنا للشراء فورًا!</span>
  <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="wa-floating-btn">
    💬
    <span class="wa-ping"></span>
  </a>
</div>

<!-- Social Proof Bar -->
<div class="social-proof-bar" id="socialProof">
  <div class="live-dot"></div>
  <span>🔥 <span id="viewers">23</span> شخص يشاهدون هذا العرض الآن</span>
</div>

<!-- Floating CTA Mobile -->
<div class="floating-cta">
  <a href="https://wa.me/9647515538709?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20%F0%9F%91%8B%20%D8%A3%D8%B1%D9%8A%D8%AF%20%D8%B4%D8%B1%D8%A7%D8%A1%20Canva%20Designer%20Power%20Bundle%20%D8%A8%D8%B3%D8%B9%D8%B1%20%241.35%20%F0%9F%8E%A8" target="_blank" class="cta-btn" style="gap:8px;">
    <span class="wa-icon">💬</span>
    اطلب عبر واتساب – \$1.35 فقط
  </a>
</div>

<script>
// WhatsApp link
const WA_LINK = "https://wa.me/9647515538709?text=" + encodeURIComponent("مرحباً 👋 أريد شراء Canva Designer Power Bundle بسعر \$1.35 🎨");

// Countdown Timer
let totalSeconds = 2 * 3600 + 47 * 60 + 33;

function updateTimer() {
  const h = Math.floor(totalSeconds / 3600);
  const m = Math.floor((totalSeconds % 3600) / 60);
  const s = totalSeconds % 60;
  
  document.getElementById('hours').textContent = String(h).padStart(2, '0');
  document.getElementById('minutes').textContent = String(m).padStart(2, '0');
  document.getElementById('seconds').textContent = String(s).padStart(2, '0');
  
  if (totalSeconds > 0) {
    totalSeconds--;
  }
}

setInterval(updateTimer, 1000);
updateTimer();

// Scroll animations
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
    }
  });
}, { threshold: 0.1 });

document.querySelectorAll('.animate-in').forEach(el => observer.observe(el));

// Viewers count
function updateViewers() {
  const base = 18;
  const variation = Math.floor(Math.random() * 15);
  document.getElementById('viewers').textContent = base + variation;
}

setInterval(updateViewers, 4000);

// Sold count increment
let soldBase = 847;
function updateSold() {
  if (Math.random() > 0.6) {
    soldBase++;
    document.getElementById('sold-count').textContent = soldBase;
  }
}
setInterval(updateSold, 8000);

// Social proof notifications
const names = ['أحمد', 'سارة', 'محمد', 'فاطمة', 'خالد', 'نورة', 'عمر', 'ليلى', 'يوسف', 'هدى', 'علي', 'مريم'];
const countries = ['🇸🇦', '🇦🇪', '🇪🇬', '🇲🇦', '🇯🇴', '🇰🇼', '🇶🇦', '🇧🇭'];

let notificationEl = null;

function showNotification() {
  if (notificationEl) {
    notificationEl.remove();
  }
  
  const name = names[Math.floor(Math.random() * names.length)];
  const country = countries[Math.floor(Math.random() * countries.length)];
  const mins = Math.floor(Math.random() * 12) + 1;
  
  notificationEl = document.createElement('div');
  notificationEl.style.cssText = `
    position: fixed;
    top: 50px;
    right: 20px;
    background: rgba(15,15,26,0.95);
    border: 1px solid rgba(37,211,102,0.4);
    border-radius: 12px;
    padding: 14px 20px;
    z-index: 1002;
    animation: slide-down 0.5s ease;
    backdrop-filter: blur(10px);
    font-family: 'Tajawal', sans-serif;
    font-size: 13px;
    color: #E5E7EB;
    max-width: 320px;
    direction: rtl;
    box-shadow: 0 8px 24px rgba(0,0,0,0.3);
  `;
  notificationEl.innerHTML = `
    <div style="display:flex; align-items:center; gap:10px;">
      <span style="font-size:20px;">${country}</span>
      <div>
        <div style="font-weight:700; color:white;">${name} اشترى الحزمة ✅</div>
        <div style="font-size:11px; color:#9CA3AF; margin-top:2px;">عبر واتساب • منذ ${mins} دقائق</div>
      </div>
    </div>
  `;
  
  const style = document.createElement('style');
  style.textContent = `@keyframes slide-down { from { transform: translateY(-30px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }`;
  notificationEl.appendChild(style);
  
  document.body.appendChild(notificationEl);
  
  setTimeout(() => {
    if (notificationEl) {
      notificationEl.style.transition = 'all 0.5s';
      notificationEl.style.opacity = '0';
      notificationEl.style.transform = 'translateY(-20px)';
      setTimeout(() => {
        if (notificationEl) notificationEl.remove();
        notificationEl = null;
      }, 500);
    }
  }, 4000);
}

setTimeout(() => showNotification(), 3000);
setInterval(showNotification, 12000);

// Pulse WhatsApp floating button periodically
setInterval(() => {
  const btn = document.querySelector('.wa-floating-btn');
  if (btn) {
    btn.style.transform = 'scale(1.15)';
    setTimeout(() => { btn.style.transform = 'scale(1)'; }, 300);
  }
}, 5000);
</script>
</body>
</html>
