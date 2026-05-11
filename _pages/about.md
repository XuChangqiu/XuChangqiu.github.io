---
permalink: /
title: "Homepage"
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
.home-section {
  margin: 34px 0 44px 0;
}

.home-title {
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 1.55rem;
  font-weight: 850;
  margin-bottom: 20px;
  color: #111827;
  letter-spacing: 0;
}

.home-title::before {
  content: attr(data-icon);
  width: 36px;
  height: 36px;
  border-radius: 12px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #fff1f2 0%, #eff6ff 100%);
  border: 1px solid #e5e7eb;
  box-shadow: 0 4px 12px rgba(15, 23, 42, 0.06);
  font-size: 1.05rem;
  flex: 0 0 auto;
}

.home-title::after {
  content: "";
  height: 1px;
  flex: 1;
  background: linear-gradient(90deg, #e5e7eb 0%, rgba(229, 231, 235, 0) 100%);
  margin-left: 4px;
}

.bio-card {
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  padding: 26px 30px;
  background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
  box-shadow: 0 8px 22px rgba(15, 23, 42, 0.05);
  margin-bottom: 30px;
}

.bio-main {
  font-size: 1.08rem;
  line-height: 1.9;
  color: #374151;
}

.tag-row {
  margin-top: 18px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.tag {
  display: inline-block;
  padding: 7px 13px;
  border-radius: 999px;
  background: #fef2f2;
  color: #991b1b;
  font-size: 0.88rem;
  font-weight: 650;
  border: 1px solid #fee2e2;
}

.action-row {
  margin-top: 22px;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.action-btn {
  display: inline-block;
  padding: 9px 15px;
  border-radius: 10px;
  text-decoration: none !important;
  font-weight: 700;
  font-size: 0.92rem;
  border: 1px solid #d1d5db;
  background: #ffffff;
  color: #374151 !important;
  box-shadow: 0 2px 6px rgba(15, 23, 42, 0.04);
}

.info-card {
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  padding: 22px 26px;
  background: #ffffff;
  box-shadow: 0 6px 18px rgba(15, 23, 42, 0.04);
}

.info-card.soft {
  background: #fafafa;
}

.edu-head {
  display: flex;
  align-items: center;
  gap: 18px;
  flex-wrap: wrap;
}

.edu-logo {
  width: 76px;
  height: 76px;
  object-fit: contain;
  border-radius: 14px;
  background: #ffffff;
  padding: 8px;
  border: 1px solid #e5e7eb;
  box-shadow: 0 3px 10px rgba(15, 23, 42, 0.06);
}

.edu-name {
  font-size: 1.18rem;
  font-weight: 800;
  color: #111827;
  margin-bottom: 6px;
}

.edu-meta {
  color: #4b5563;
  margin-bottom: 14px;
  font-size: 0.98rem;
}

.edu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
  gap: 12px;
  margin-top: 18px;
}

.edu-item {
  padding: 12px 14px;
  border-radius: 12px;
  background: #f8fafc;
  border: 1px solid #eef2f7;
}

.pub-card {
  border-radius: 18px;
  padding: 24px 28px;
  margin: 22px 0;
  background: #f8fafc;
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.055);
  border: 1px solid #e5e7eb;
  position: relative;
  overflow: hidden;
}

.pub-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 6px;
  height: 100%;
}

.pub-card.med::before {
  background: #10b981;
}

.pub-card.cv::before {
  background: #4f46e5;
}

.pub-card.rs::before {
  background: #0ea5e9;
}

.pub-label {
  display: inline-block;
  padding: 5px 10px;
  border-radius: 999px;
  font-size: 0.78rem;
  font-weight: 800;
  margin-bottom: 12px;
}

.pub-label.med {
  background: #dcfce7;
  color: #047857;
}

.pub-label.cv {
  background: #eef2ff;
  color: #3730a3;
}

.pub-label.rs {
  background: #e0f2fe;
  color: #0369a1;
}

.pub-title {
  font-size: 1.18rem;
  font-weight: 850;
  color: #111827;
  line-height: 1.45;
  margin-bottom: 10px;
}

.pub-authors {
  line-height: 1.75;
  color: #374151;
  margin-bottom: 6px;
}

.pub-venue {
  font-style: italic;
  color: #4b5563;
  margin-bottom: 14px;
}

.pub-short {
  line-height: 1.85;
  color: #374151;
}

.pub-figure {
  margin: 18px auto 14px auto;
  max-width: 900px;
}

.pub-figure.multi {
  display: grid;
  gap: 14px;
}

.pub-figure img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 14px;
  border: 1px solid #e5e7eb;
  background: #ffffff;
  box-shadow: 0 6px 18px rgba(15, 23, 42, 0.06);
}

.detail-box .pub-figure {
  max-width: 760px;
  margin: 18px auto 0;
}

.metric-row {
  margin-top: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.metric {
  display: inline-block;
  padding: 6px 11px;
  border-radius: 10px;
  font-size: 0.86rem;
  font-weight: 800;
  background: #ffffff;
  border: 1px solid #e5e7eb;
  color: #374151;
}

details {
  margin-top: 14px;
}

summary {
  cursor: pointer;
  font-weight: 800;
  color: #2563eb;
  margin-top: 10px;
}

.detail-box {
  margin-top: 12px;
  padding: 15px 18px;
  border-radius: 12px;
  background: #ffffff;
  border: 1px solid #e5e7eb;
  line-height: 1.85;
  color: #374151;
}

.project-card {
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  padding: 24px 28px;
  background: #ffffff;
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.045);
}

.project-title {
  font-size: 1.16rem;
  font-weight: 850;
  margin-bottom: 8px;
  color: #111827;
}

.project-meta {
  color: #4b5563;
  font-style: italic;
  margin-bottom: 14px;
}

.award-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(285px, 1fr));
  gap: 14px;
  margin-top: 18px;
}

.award-card {
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  padding: 17px 18px;
  background: #fafafa;
  box-shadow: 0 5px 14px rgba(15, 23, 42, 0.035);
}

.award-name {
  font-weight: 850;
  color: #111827;
  margin-bottom: 6px;
}

.award-meta {
  color: #4b5563;
  line-height: 1.7;
}

@media (max-width: 768px) {
  .bio-card,
  .info-card,
  .pub-card,
  .project-card {
    padding: 20px 18px;
  }
}
</style>

<div class="bio-card" id="about">
  <div class="bio-main">
    Hi! I am <strong>Changqiu Xu</strong> (Chinese name: <strong>徐长秋</strong>), an undergraduate student majoring in <strong>Internet of Things Engineering</strong> at <strong>Henan University of Economics and Law</strong>. My current research interests lie in medical image restoration and sparse-view 3D-DSA reconstruction, with a focus on deep learning methods for structure-preserving image enhancement and reconstruction.
  </div>

  <div class="tag-row">
    <span class="tag">Sparse-view 3D-DSA Reconstruction</span>
    <span class="tag">Medical Image Restoration</span>
    <span class="tag">Deep Learning</span>
    <span class="tag">Computer Vision</span>
  </div>

  <div class="action-row">
    <a class="action-btn" href="mailto:17303839670@163.com">Email</a>
    <a class="action-btn" href="https://github.com/XuChangqiu">GitHub</a>
  </div>
</div>

<div class="home-section" id="education">
  <div class="home-title" data-icon="🎓">Education</div>

  <div class="info-card soft">
    <div class="edu-head">
      <img class="edu-logo" src="/images/huel-logo.png" alt="Henan University of Economics and Law Logo">

      <div>
        <div class="edu-name">Henan University of Economics and Law</div>
        <div class="edu-meta">B.Eng. Candidate in Internet of Things Engineering &nbsp; | &nbsp; Sep. 2023 - Jun. 2027</div>
      </div>
    </div>

    <div class="edu-grid">
      <div class="edu-item">
        <strong>GPA</strong><br>
        3.90
      </div>

      <div class="edu-item">
        <strong>Ranking</strong><br>
        1 / 40
      </div>

      <div class="edu-item">
        <strong>English</strong><br>
        CET-4: 505
      </div>
    </div>
  </div>
</div>

<div class="home-section" id="publications">
  <div class="home-title" data-icon="📚">Publications</div>

  <div class="pub-card med">
    <div class="pub-label med">Medical Imaging · 3D-DSA</div>

    <div class="pub-title">
      Vascular Morphology Motivated Progressive Structure-Enhanced Restoration for Sparse-view 3D-DSA
    </div>

    <div class="pub-authors">
      Yikun Zhang, <strong>Changqiu Xu</strong>, Shiyu Zhu, Weilong Mao, Jun Xiang, Rongjun Ge, Jian Yang, Yang Chen
    </div>

    <div class="pub-venue">
      IEEE Journal of Biomedical and Health Informatics (CAS Q1 / 中科院一区), major revision
    </div>

    <div class="pub-short">
      A progressive structure-enhanced restoration framework for sparse-view 3D-DSA that combines coarse 3D restoration and fine 2.5D refinement to suppress artifacts and recover vascular continuity.
    </div>

    <div class="metric-row">
      <span class="metric">CAS Q1 / 中科院一区</span>
      <span class="metric">Major Revision</span>
      <span class="metric">Student First Author</span>
      <a class="metric" href="https://github.com/DarkBreakerZero/PSER">Code</a>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        This work targets severe streak artifacts and vascular structure degradation in sparse-view 3D-DSA. The framework first performs coarse 3D restoration with weighted convolution and wavelet-domain enhancement, then applies a 2.5D refinement network with dynamic snake convolution to better preserve tortuous vascular structures and fine vessel continuity.
        <div class="pub-figure multi">
          <img src="/images/publications/pser-fig1.jpg" alt="PSER vascular morphology motivation">
          <img src="/images/publications/pser-fig3.jpg" alt="PSER network architecture">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card med">
    <div class="pub-label med">Medical Imaging · DSA</div>

    <div class="pub-title">
      DSANet: Dynamic Snake Convolution Attention Network for Coarse-to-Fine DSA Imaging using Pseudo Aligned Dataset
    </div>

    <div class="pub-authors">
      Shiyu Zhu, <strong>Changqiu Xu</strong>, Weilong Mao, Jun Xiang, Rongjun Ge, Yikun Zhang, Yang Chen
    </div>

    <div class="pub-venue">
      IEEE Journal of Biomedical and Health Informatics (CAS Q1 / 中科院一区), under review
    </div>

    <div class="pub-short">
      A coarse-to-fine DSA imaging network that uses pseudo aligned data and dynamic snake convolution attention to suppress motion artifacts while preserving vascular structure.
    </div>

    <div class="metric-row">
      <span class="metric">CAS Q1 / 中科院一区</span>
      <span class="metric">Under Review</span>
      <span class="metric">Second Author</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        DSANet addresses motion artifacts caused by misalignment between mask and live images in DSA imaging. It uses a coarse-to-fine pipeline: an initial DSA imaging stage generates preliminary vessel images, and a pseudo aligned dataset is then constructed to train a dynamic snake convolution attention network for artifact suppression and vessel detail preservation.
        <div class="pub-figure multi">
          <img src="/images/publications/dsanet-fig1.jpg" alt="DSANet coarse-to-fine imaging framework">
          <img src="/images/publications/dsanet-fig2-v2.jpg" alt="DSANet dynamic snake convolution attention architecture">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card med">
    <div class="pub-label med">Medical Imaging · Sparse-view Reconstruction</div>

    <div class="pub-title">
      PDAO-Net: A Physics-Constrained Dual-Domain Alternating Optimization Network for Sparse-View 3D-DSA Reconstruction
    </div>

    <div class="pub-authors">
      <strong>Changqiu Xu</strong>, Xi Wang, Yujia Li, Tong Liang, Kang Yang, Longfei Xiao, Yikun Zhang, Yang Chen
    </div>

    <div class="pub-venue">
      International Conference on Neural Information Processing (ICONIP), 2026 (CCF C), under review
    </div>

    <div class="pub-short">
      A physics-constrained dual-domain reconstruction framework that alternates between projection-domain correction and image-domain refinement for sparse-view 3D-DSA reconstruction.
    </div>

    <div class="metric-row">
      <span class="metric">CCF C</span>
      <span class="metric">Under Review</span>
      <span class="metric">First Author</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        PDAO-Net formulates sparse-view 3D-DSA reconstruction as a dual-domain alternating optimization process. It combines projection-domain correction, image-domain refinement, and measured-view replacement to enforce physical consistency while recovering small vascular branches and maintaining vessel continuity under incomplete angular sampling.
        <div class="pub-figure">
          <img src="/images/publications/pdao-net.jpg" alt="PDAO-Net framework">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card cv">
    <div class="pub-label cv">Semantic Segmentation · Mamba</div>

    <div class="pub-title">
      StructMamba-Seg: Boundary-Context Guided Deformable Scan for Semantic Segmentation
    </div>

    <div class="pub-authors">
      Longfei Xiao, Linlin Zhang, Kang Yang, <strong>Changqiu Xu</strong>, Shuyu Liu, Jianfang Wang
    </div>

    <div class="pub-venue">
      International Conference on Neural Information Processing (ICONIP), 2026 (CCF C), under review
    </div>

    <div class="pub-short">
      A structure-sensitive Mamba model for semantic segmentation that adapts scan control to boundaries, small objects, fine structures, and ambiguous regions.
    </div>

    <div class="metric-row">
      <span class="metric">CCF C</span>
      <span class="metric">Under Review</span>
      <span class="metric">Fourth Author</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        StructMamba-Seg introduces Boundary-Context Guided Deformable Scan into a Mamba-based segmentation framework. The method uses local features, boundary prompts, and multi-scale context to adapt scan positions and ordering to segmentation-specific structures such as boundaries, small objects, thin regions, and ambiguous areas.
        <div class="pub-figure">
          <img src="/images/publications/structmamba.jpg" alt="StructMamba-Seg architecture">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Remote Sensing · Low-light Enhancement</div>

    <div class="pub-title">
      Towards High-quality Low-Light Remote Sensing Image Enhancement via Geometric and Semantic Prior Guidance
    </div>

    <div class="pub-authors">
      Kang Yang, Jiaqi Zhang, <strong>Changqiu Xu</strong>, Longfei Xiao, Tong Liang, Zesheng Zhang
    </div>

    <div class="pub-venue">
      International Conference on Neural Information Processing (ICONIP), 2026 (CCF C), under review
    </div>

    <div class="pub-short">
      A low-light remote sensing image enhancement framework that introduces geometric and semantic priors to improve high-quality restoration under weak illumination.
    </div>

    <div class="metric-row">
      <span class="metric">CCF C</span>
      <span class="metric">Under Review</span>
      <span class="metric">Third Author</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        This work focuses on low-light remote sensing image enhancement, where weak illumination and sensor noise can damage both radiometry and semantic structure. The method introduces geometric and semantic priors to guide restoration, aiming to recover visually faithful images while preserving land-cover boundaries and high-level scene information.
        <div class="pub-figure">
          <img src="/images/publications/gspnet.jpg" alt="GSPNet framework">
        </div>
      </div>
    </details>
  </div>
</div>

<div class="home-section" id="research-project">
  <div class="home-title" data-icon="🔬">Project</div>

  <div class="project-card">
    <div class="project-title">
      AlgoVerse: A Personalized Programming Learning Platform Powered by Large Language Models
    </div>

    <div class="project-meta">
      Project Leader &nbsp; | &nbsp; Nov. 2024 - Jul. 2025
    </div>

    <div style="line-height: 1.9; color: #374151;">
      AlgoVerse is a personalized programming learning platform built with <strong>Vue3</strong>, <strong>Spring Boot</strong>, <strong>Docker</strong>, and <strong>PostgreSQL</strong>. The system integrates problem recommendation, process mining, learning risk prediction, AI-assisted code evaluation, anti-cheating workflows, knowledge graphs, and ECharts-based learning analytics.
    </div>

    <div class="metric-row">
      <a class="metric" href="https://github.com/XuChangqiu/huel-oj-remake-master">Code</a>
      <span class="metric">National Second Prize</span>
      <span class="metric">AI-assisted Programming Education</span>
    </div>
  </div>
</div>

<div class="home-section" id="awards">
  <div class="home-title" data-icon="🏆">Awards</div>

  <div class="award-grid">
    <div class="award-card">
      <div class="award-name">National Second Prize</div>
      <div class="award-meta">
        China Collegiate Computing Design Competition
      </div>
    </div>

    <div class="award-card">
      <div class="award-name">EI Conference Publication</div>
      <div class="award-meta">
        Research output in conference proceedings
      </div>
    </div>

    <div class="award-card">
      <div class="award-name">University Honors</div>
      <div class="award-meta">
        Merit Student<br>
        First-Class Scholarship<br>
        National Encouragement Scholarship
      </div>
    </div>
  </div>
</div>
