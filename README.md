<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Janhavi Landge | Data Scientist & AI Engineer</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Portfolio of Janhavi Landge - Data Scientist, Machine Learning & AI Engineer." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
    rel="stylesheet"
  />
  <style>
    :root {
      --bg: #050816;
      --bg-alt: #0b1020;
      --card-bg: #111827;
      --accent: #ff4b4b;
      --accent-soft: rgba(255, 75, 75, 0.15);
      --text: #e5e7eb;
      --muted: #9ca3af;
      --border: #1f2937;
      --radius-lg: 18px;
      --radius-md: 10px;
      --shadow-soft: 0 18px 40px rgba(0, 0, 0, 0.45);
      --max-width: 1050px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Poppins", system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
      background: radial-gradient(circle at top left, #1f2937 0, #050816 45%);
      color: var(--text);
      line-height: 1.7;
      -webkit-font-smoothing: antialiased;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    img {
      max-width: 100%;
      display: block;
    }

    .page {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 28px 18px 50px;
    }

    header {
      text-align: center;
      margin-bottom: 32px;
    }

    .avatar-gif {
      width: 110px;
      margin: 0 auto 10px;
      border-radius: 999px;
      box-shadow: 0 0 0 3px rgba(255, 255, 255, 0.04), var(--shadow-soft);
    }

    .headline {
      font-size: 2rem;
      font-weight: 700;
      letter-spacing: 0.03em;
    }

    .headline span {
      color: var(--accent);
    }

    .subheadline {
      font-size: 0.98rem;
      color: var(--muted);
      margin-top: 4px;
    }

    .pill {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: rgba(15, 23, 42, 0.9);
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.35);
      padding: 4px 12px;
      font-size: 0.78rem;
      color: var(--muted);
      margin-top: 12px;
    }

    .pill-dot {
      width: 8px;
      height: 8px;
      border-radius: 999px;
      background: #22c55e;
      box-shadow: 0 0 10px rgba(34, 197, 94, 0.9);
    }

    /* Layout */
    .grid-main {
      display: grid;
      grid-template-columns: minmax(0, 3fr);
      gap: 18px;
    }

    @media (min-width: 900px) {
      .grid-main {
        grid-template-columns: minmax(0, 2.2fr) minmax(0, 1.2fr);
        align-items: flex-start;
      }
    }

    /* Cards */
    .card {
      background: linear-gradient(145deg, rgba(15, 23, 42, 0.96), rgba(15, 23, 42, 0.98));
      border-radius: var(--radius-lg);
      border: 1px solid rgba(55, 65, 81, 0.9);
      padding: 18px 18px 16px;
      box-shadow: var(--shadow-soft);
      position: relative;
      overflow: hidden;
    }

    .card::before {
      content: "";
      position: absolute;
      inset: -40%;
      opacity: 0.09;
      background:
        radial-gradient(circle at 0% 0%, rgba(248, 113, 113, 0.7), transparent 55%),
        radial-gradient(circle at 90% 20%, rgba(56, 189, 248, 0.45), transparent 55%);
      pointer-events: none;
    }

    .card-inner {
      position: relative;
      z-index: 1;
    }

    .section-title {
      font-size: 1.08rem;
      font-weight: 600;
      margin-bottom: 10px;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .section-title span.icon {
      font-size: 1.2rem;
    }

    .section-sub {
      font-size: 0.87rem;
      color: var(--muted);
      margin-bottom: 6px;
    }

    p {
      font-size: 0.9rem;
      color: #e5e7eb;
    }

    /* Links & badges */
    .link-row {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 9px;
    }

    .btn-link {
      font-size: 0.8rem;
      border-radius: 999px;
      padding: 7px 13px;
      display: inline-flex;
      align-items: center;
      gap: 7px;
      border: 1px solid rgba(148, 163, 184, 0.6);
      background: rgba(15, 23, 42, 0.85);
      cursor: pointer;
      transition: all 0.18s ease-out;
    }

    .btn-link:hover {
      border-color: var(--accent);
      background: rgba(248, 113, 113, 0.16);
      transform: translateY(-1px);
    }

    .btn-link span.icon {
      font-size: 1rem;
    }

    .pill-soft {
      display: inline-flex;
      align-items: center;
      padding: 3px 9px;
      border-radius: 999px;
      background: rgba(31, 41, 55, 0.85);
      font-size: 0.78rem;
      color: var(--muted);
      border: 1px solid rgba(55, 65, 81, 0.9);
      gap: 6px;
      margin-top: 10px;
    }

    .pill-soft strong {
      font-weight: 600;
      color: #f9fafb;
    }

    /* Tech grid */
    .tech-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(190px, 1fr));
      gap: 10px;
      margin-top: 10px;
    }

    .tech-item {
      background: rgba(15, 23, 42, 0.95);
      border-radius: var(--radius-md);
      border: 1px solid rgba(55, 65, 81, 0.9);
      padding: 10px 11px;
      font-size: 0.8rem;
    }

    .tech-item-title {
      font-weight: 600;
      margin-bottom: 4px;
      font-size: 0.8rem;
    }

    .tech-item-body {
      color: var(--muted);
      font-size: 0.8rem;
    }

    /* Projects & tables */
    .projects-section {
      margin-top: 12px;
    }

    .projects-group {
      margin-bottom: 16px;
    }

    .projects-heading {
      font-size: 0.95rem;
      font-weight: 600;
      margin-bottom: 6px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .projects-heading span.icon {
      font-size: 1rem;
    }

    .projects-note {
      font-size: 0.8rem;
      color: var(--muted);
      margin-bottom: 6px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.8rem;
      margin-top: 4px;
    }

    th, td {
      padding: 7px 8px;
      text-align: left;
      border-bottom: 1px solid rgba(31, 41, 55, 0.95);
      vertical-align: top;
    }

    th {
      font-weight: 600;
      color: #9ca3af;
      font-size: 0.78rem;
    }

    tr:last-child td {
      border-bottom: none;
    }

    tbody tr:hover td {
      background: rgba(15, 23, 42, 0.9);
    }

    .repo-link {
      font-weight: 500;
      color: #e5e7eb;
    }

    .repo-link span {
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      opacity: 0.65;
    }

    .tag {
      display: inline-flex;
      align-items: center;
      border-radius: 999px;
      padding: 2px 7px;
      border: 1px solid rgba(148, 163, 184, 0.4);
      font-size: 0.72rem;
      color: var(--muted);
      margin-right: 5px;
      margin-top: 3px;
    }

    .badges-row {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 10px;
    }

    .badges-row img {
      height: 26px;
      border-radius: 999px;
    }

    footer {
      text-align: center;
      margin-top: 26px;
      font-size: 0.78rem;
      color: var(--muted);
      padding-top: 10px;
      border-top: 1px solid rgba(31, 41, 55, 0.95);
    }

    .accent-text {
      color: var(--accent);
      font-weight: 600;
    }
  </style>
</head>
<body>
  <div class="page">
    <header>
      <img
        src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif"
        alt="Developer GIF"
        class="avatar-gif"
      />
      <div class="headline">👋 Hello, I'm <span>Janhavi Landge</span></div>
      <div class="subheadline">
        Data Scientist · Machine Learning Engineer · AI & GenAI Specialist
      </div>
      <div class="pill">
        <span class="pill-dot"></span>
        Open to roles in <strong>Data Science, ML/DL & AI Engineering</strong>
      </div>
    </header>

    <main class="grid-main">
      <!-- LEFT: About + Projects -->
      <section class="card">
        <div class="card-inner">
          <h2 class="section-title">
            <span class="icon">🚀</span> About Me
          </h2>
          <p>
            I am a highly motivated and results-driven
            <span class="accent-text">Data Scientist & AI Engineer</span> with hands-on experience
            in <strong>Machine Learning, Deep Learning, NLP, Computer Vision, Generative AI, Time Series Forecasting,</strong>
            and <strong>MLOps</strong>.
            I enjoy taking projects from <strong>raw data</strong> all the way to
            <strong>production-ready models, dashboards, and intelligent applications</strong>.
          </p>

          <div class="section-sub" style="margin-top: 12px;">Connect with Me</div>
          <div class="link-row">
            <a href="https://www.linkedin.com/in/janhavi-landge-7a1072276/" class="btn-link" target="_blank" rel="noreferrer">
              <span class="icon">💼</span>
              <span>LinkedIn</span>
            </a>
            <a href="https://github.com/janhavilandge21" class="btn-link" target="_blank" rel="noreferrer">
              <span class="icon">🐙</span>
              <span>GitHub</span>
            </a>
            <a href="mailto:janhavilandge2@gmail.com" class="btn-link">
              <span class="icon">✉️</span>
              <span>Email</span>
            </a>
          </div>

          <div class="pill-soft">
            <span>🎯</span>
            <span>Goal: Secure a role as a <strong>Data Scientist / ML Engineer / AI Developer</strong></span>
          </div>

          <!-- Tech Stack -->
          <h2 class="section-title" style="margin-top: 18px;">
            <span class="icon">🧪</span> Technical Stack
          </h2>
          <p class="section-sub">
            A strong end-to-end stack from data exploration to deployment and automation.
          </p>

          <div class="tech-grid">
            <div class="tech-item">
              <div class="tech-item-title">Languages</div>
              <div class="tech-item-body">
                Python (Advanced), SQL, R (Foundational)
              </div>
            </div>
            <div class="tech-item">
              <div class="tech-item-title">Machine Learning</div>
              <div class="tech-item-body">
                Scikit-learn, Feature Engineering, Classification, Regression, Time Series, Model Tuning
              </div>
            </div>
            <div class="tech-item">
              <div class="tech-item-title">Deep Learning & AI</div>
              <div class="tech-item-body">
                TensorFlow, Keras, Hugging Face, Transformers, NLP, Computer Vision, GenAI
              </div>
            </div>
            <div class="tech-item">
              <div class="tech-item-title">Data & BI</div>
              <div class="tech-item-body">
                Pandas, NumPy, Power BI, Matplotlib, Seaborn, Streamlit, MySQL
              </div>
            </div>
            <div class="tech-item">
              <div class="tech-item-title">MLOps & DevOps</div>
              <div class="tech-item-body">
                CI/CD, GitHub Actions, Testing Pipelines, Model Deployment, Git/GitHub
              </div>
            </div>
            <div class="tech-item">
              <div class="tech-item-title">Other Tools</div>
              <div class="tech-item-body">
                OpenCV, YOLO (Ultralytics), Web Scraping (Requests, BeautifulSoup, Selenium)
              </div>
            </div>
          </div>

          <div class="badges-row">
            <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python Badge" />
            <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn Badge" />
            <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow Badge" />
            <img src="https://img.shields.io/badge/Hugging%20Face-FFD21C?style=for-the-badge&logo=huggingface&logoColor=black" alt="Hugging Face Badge" />
            <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="PowerBI Badge" />
            <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit Badge" />
            <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV Badge" />
            <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL Badge" />
          </div>
        </div>
      </section>

      <!-- RIGHT: Projects grouped -->
      <section class="card">
        <div class="card-inner">
          <h2 class="section-title">
            <span class="icon">💡</span> Portfolio by Domain
          </h2>
          <p class="section-sub">
            A curated selection of my work across AI, ML/DL, GenAI, Vision, Analytics, and MLOps.
          </p>

          <div class="projects-section">

            <!-- AI & GenAI -->
            <div class="projects-group">
              <div class="projects-heading">
                <span class="icon">🤖</span>
                Artificial Intelligence, NLP & Generative AI
              </div>
              <p class="projects-note">
                End-to-end intelligent systems using LLMs, transformers, agents, and advanced NLP.
              </p>
              <table>
                <thead>
                  <tr>
                    <th>Project Repository</th>
                    <th>Impact Summary</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Genrative-Ai" class="repo-link" target="_blank" rel="noreferrer">
                        Genrative-Ai
                      </a>
                      <div class="tag">LLMs</div>
                      <div class="tag">RAG</div>
                      <div class="tag">Embeddings</div>
                    </td>
                    <td>
                      Hands-on implementation of <strong>LLM workflows</strong> including prompt engineering,
                      vector search, embeddings, and retrieval-augmented generation for real-world tasks.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Agentic-Ai" class="repo-link" target="_blank" rel="noreferrer">
                        Agentic-Ai
                      </a>
                      <div class="tag">AI Agents</div>
                      <div class="tag">Tool Use</div>
                    </td>
                    <td>
                      Building <strong>agentic AI systems</strong> capable of planning, tool usage, and reasoning,
                      leveraging frameworks like LangChain/agents and modern LLM APIs.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/HUGGINGFACE" class="repo-link" target="_blank" rel="noreferrer">
                        HUGGINGFACE
                      </a>
                      <div class="tag">Transformers</div>
                      <div class="tag">Fine-tuning</div>
                    </td>
                    <td>
                      Demonstrates the use of <strong>Hugging Face Transformers</strong> for text classification,
                      summarization, and other NLP tasks with pre-trained and fine-tuned models.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Natural-Language-Processing" class="repo-link" target="_blank" rel="noreferrer">
                        Natural-Language-Processing
                      </a>
                      <div class="tag">NLP</div>
                      <div class="tag">Text Analytics</div>
                    </td>
                    <td>
                      Covers complete NLP pipelines: data cleaning, tokenization, feature engineering,
                      sentiment analysis, topic modeling, and traditional ML-based NLP solutions.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Gen-AI-Robort-Visualization-Dashboard" class="repo-link" target="_blank" rel="noreferrer">
                        Gen-AI-Robort-Visualization-Dashboard
                      </a>
                      <div class="tag">GenAI</div>
                      <div class="tag">Dashboard</div>
                    </td>
                    <td>
                      Integrates <strong>Generative AI</strong> models with interactive dashboards for real-time
                      visualization and conversational insights, showcasing AI-assisted analytics.
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>

            <!-- Vision -->
            <div class="projects-group">
              <div class="projects-heading">
                <span class="icon">👁️</span>
                Computer Vision & Object Detection
              </div>
              <p class="projects-note">
                Image understanding, object detection and visual intelligence with DL & OpenCV.
              </p>
              <table>
                <thead>
                  <tr>
                    <th>Project Repository</th>
                    <th>Impact Summary</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Ultralytics_YOLO" class="repo-link" target="_blank" rel="noreferrer">
                        Ultralytics_YOLO
                      </a>
                      <div class="tag">YOLO</div>
                      <div class="tag">Object Detection</div>
                    </td>
                    <td>
                      Implements <strong>YOLO-based object detection</strong> pipelines including dataset handling,
                      model training, evaluation, and inference for real-time detection tasks.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Computer-Vision" class="repo-link" target="_blank" rel="noreferrer">
                        Computer-Vision
                      </a>
                      <div class="tag">OpenCV</div>
                      <div class="tag">Image Processing</div>
                    </td>
                    <td>
                      Projects on <strong>image processing, feature extraction, segmentation, and classification</strong>
                      using OpenCV and deep learning models for real-world vision problems.
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>

            <!-- ML & DL -->
            <div class="projects-group">
              <div class="projects-heading">
                <span class="icon">📈</span>
                Machine Learning & Deep Learning
              </div>
              <p class="projects-note">
                From classical ML models to advanced neural networks and time series forecasting.
              </p>
              <table>
                <thead>
                  <tr>
                    <th>Project Repository</th>
                    <th>Impact Summary</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Machine-Learning-Project" class="repo-link" target="_blank" rel="noreferrer">
                        Machine-Learning-Project
                      </a>
                      <div class="tag">End-to-End ML</div>
                    </td>
                    <td>
                      End-to-end ML projects covering <strong>data preprocessing, feature engineering, model selection,
                      hyperparameter tuning,</strong> and comprehensive evaluation.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Deep-Learning-Projects" class="repo-link" target="_blank" rel="noreferrer">
                        Deep-Learning-Projects
                      </a>
                      <div class="tag">Neural Networks</div>
                    </td>
                    <td>
                      Collection of deep learning projects using <strong>TensorFlow/Keras</strong> for classification,
                      sequence modeling, and other advanced tasks.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Iris-Flower-Classification" class="repo-link" target="_blank" rel="noreferrer">
                        Iris-Flower-Classification
                      </a>
                      <div class="tag">Classification</div>
                    </td>
                    <td>
                      Classic ML classification problem achieving around <strong>97% precision</strong>,
                      demonstrating solid understanding of ML pipelines and evaluation.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Time-Series-Forcastinghttps" class="repo-link" target="_blank" rel="noreferrer">
                        Time-Series-Forcasting
                      </a>
                      <div class="tag">Time Series</div>
                      <div class="tag">Forecasting</div>
                    </td>
                    <td>
                      <strong>Time series forecasting</strong> using methods like ARIMA, Prophet, and LSTM to
                      predict trends and support data-driven business decisions.
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>

            <!-- Data Analytics & BI -->
            <div class="projects-group">
              <div class="projects-heading">
                <span class="icon">📊</span>
                Data Analytics, Dashboards & Business Intelligence
              </div>
              <p class="projects-note">
                Turning raw data into insights, dashboards, and executive-ready reports.
              </p>
              <table>
                <thead>
                  <tr>
                    <th>Project Repository</th>
                    <th>Impact Summary</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Power--BI-Project" class="repo-link" target="_blank" rel="noreferrer">
                        Power--BI-Project
                      </a>
                      <div class="tag">Power BI</div>
                      <div class="tag">Dashboards</div>
                    </td>
                    <td>
                      End-to-end <strong>Power BI dashboards</strong> converting complex datasets into
                      interactive reports with KPIs, filters, and drill-down analytics.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Emp-Performance-Dashboard" class="repo-link" target="_blank" rel="noreferrer">
                        Emp-Performance-Dashboard
                      </a>
                      <div class="tag">HR Analytics</div>
                    </td>
                    <td>
                      Employee performance dashboard with <strong>KPI tracking, aggregations, and trends</strong>,
                      built using Power BI / Streamlit and clean data modeling.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Exploratory-Data-Analysis" class="repo-link" target="_blank" rel="noreferrer">
                        Exploratory-Data-Analysis
                      </a>
                      <div class="tag">EDA</div>
                    </td>
                    <td>
                      Advanced EDA projects focusing on <strong>outlier detection, feature insights, and statistical
                      analysis</strong> to guide business decisions.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Data-Visualization-With-Matplotlib" class="repo-link" target="_blank" rel="noreferrer">
                        Data-Visualization-With-Matplotlib
                      </a>
                      <div class="tag">Visualization</div>
                    </td>
                    <td>
                      A set of visual storytelling projects using <strong>Matplotlib and Seaborn</strong>
                      to communicate patterns and trends clearly.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Retail-Data-Analysis" class="repo-link" target="_blank" rel="noreferrer">
                        Retail-Data-Analysis
                      </a>
                      <div class="tag">Retail Analytics</div>
                    </td>
                    <td>
                      In-depth analysis of retail data to uncover <strong>sales patterns, customer segments, and inventory
                      optimization strategies</strong>.
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>

            <!-- Data Engineering & MLOps -->
            <div class="projects-group">
              <div class="projects-heading">
                <span class="icon">⚙️</span>
                Data Engineering, Automation & MLOps
              </div>
              <p class="projects-note">
                Deployable, maintainable, and automated data & ML pipelines.
              </p>
              <table>
                <thead>
                  <tr>
                    <th>Project Repository</th>
                    <th>Impact Summary</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/CICD-Testing" class="repo-link" target="_blank" rel="noreferrer">
                        CICD-Testing
                      </a>
                      <div class="tag">CI/CD</div>
                      <div class="tag">MLOps</div>
                    </td>
                    <td>
                      Showcases <strong>CI/CD pipelines</strong> for ML projects with automated testing and deployment
                      using Git/GitHub workflows and best practices.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Web-Scrapping" class="repo-link" target="_blank" rel="noreferrer">
                        Web-Scrapping
                      </a>
                      <div class="tag">Web Scraping</div>
                      <div class="tag">Automation</div>
                    </td>
                    <td>
                      Automated <strong>web data extraction</strong> using BeautifulSoup, Requests, and Selenium
                      to build datasets for analytics and ML applications.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/SQL-Project" class="repo-link" target="_blank" rel="noreferrer">
                        SQL-Project
                      </a>
                      <div class="tag">SQL</div>
                      <div class="tag">Data Warehousing</div>
                    </td>
                    <td>
                      Complex SQL queries, joins, aggregations, and schema design for <strong>analytics and reporting</strong>
                      with a strong focus on performance.
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <a href="https://github.com/janhavilandge21/Comparison-of-SQL-and-Python-Pandas-" class="repo-link" target="_blank" rel="noreferrer">
                        Comparison-of-SQL-and-Python-Pandas-
                      </a>
                      <div class="tag">SQL vs Pandas</div>
                    </td>
                    <td>
                      Comparative analysis of <strong>SQL vs Pandas</strong> for data manipulation, evaluating performance,
                      efficiency, and use cases for each tool.
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>

          </div>
        </div>
      </section>
    </main>

    <footer>
      Crafted by Janhavi Landge · Data Science & AI | GitHub:
      <a href="https://github.com/janhavilandge21" target="_blank" rel="noreferrer">janhavilandge21</a>
    </footer>
  </div>
</body>
</html>
