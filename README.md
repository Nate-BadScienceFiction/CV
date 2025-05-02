# CV
**Nate Combs**
(Last updated 5/6/2025)

Selected technical posts and projects demonstrate my versatility in CI/CD engineering, system integration and testing, and cross-language prototyping (Python, JavaScript, C++). Each reflects a hands-on, solutions-focused approach—built under live CI constraints, with real-time debugging across diverse tech stacks.

Much of this work was pair-programmed with large language models from OpenAI and Anthropic—tireless collaborators throughout.

---
**Motivations:**

1. *Research* - Generative AI for [pair programming](https://en.wikipedia.org/wiki/Pair_programming).
2. *Evaluation* - Application prototyping.
3. *Exploration* - Tech-stack education.

---
**Highlights:**

🔹 **FastAPI Thin Client Architecture**
Architected a modular FastAPI backend for serving visualizations and API endpoints to JavaScript-based thin clients. The clean separation of concerns supports targeted CI testing, scalable endpoint validation, and rapid UI iteration.

🔹 **LLM-Aided CI Troubleshooting**
Used chain-of-thought prompt design with OpenAI models (o1, o3-mini) to debug ∼2,000-line GitHub Actions logs and fix downstream Pyparsing failures in a PDF parser pipeline: integrated regression testing and hardened parser logic.

🔹 **Cloud-Based LLM Prototyping**
Automated spin-up of GPU-backed AWS EC2 (g4dn) instances with WSL2 remote workflows. Used SSH/SCP scripting to prototype and train models on hosted NVIDIA environments, minimizing cost with rent-by-hour strategies.

🔹 **CI/CD YAML Engineering [1]**
Built GitHub Actions workflows for Python testing, static analysis (black, flake8, mypy), and OpenAI key injection via GitHub Secrets. Implemented fallback logic, caching strategies, and prompt-driven diagnostics to repair broken workflows.

🔹 **Pervasive LLM‑driven automation**
Used LLMs to auto-generate CI-integrated diagrams, C++ UI modules, Python/C++ [sentiment‑analysis tools], and even YAML fragments. Explored “brief-driven” prompt engineering to structure test scaffolds in DevOps workflows.

🔹 **Redis + Embedding Cache for CI Cost Control**
Integrated Redis vector DBs with SHA-256 deduplication to cache OpenAI embeddings. Reduced API calls and streamlined CI inference loops using fallback patterns for Redis downtimes.

🔹 **SysML & LaTeX Artifact Generation**
Orchestrated multi-repo GitHub Actions to auto-generate architecture diagrams and SysML reports via Graphviz/LaTeX Actions in GitHub workflows. Integrated fallback behaviors to render raw PDFs when CI rendering fails.

🔹 **Local LLM Dev with Ollama**
Provisioned reproducible LLM dev environments using Ollama on WSL2 to host Llama2 (7B) locally. Integrated VS Code for debugging prompt chains, eliminating API costs and improving test-cycle speed.

🔹 **SonarQube CI/CD Static Analysis [1]**
Containerized SonarQube with WSL2 and Docker for scalable local testing. Integrated scans into GitHub Actions to detect code smells.

For the complete archive of technical posts:

📘 [Substack Articles](https://natecombs.substack.com/)

📘 [Medium Writings](https://medium.com/me/stories/public)

---
**Keywords:**
1. CI/CD pipelines [1]
2. GitHub Actions
3. Docker
4. Containerization
5. AWS EC2
6. AMI selection
7. Cost optimization
8. Infrastructure provisioning
9. WSL2 integration
10. SSH/SCP
11. FastAPI
12. REST API design
13. Automated testing
14. Unit‑test automation
15. Regression testing
16. Dependency management
17. Caching strategies
18. Matrix testing
19. Style‑check integration (black, flake8, mypy)
20. SonarQube
21. Logging & observability
22. Error handling & fallback logic
23. Pipeline resilience
24. Repository\_dispatch (cross‑repo triggers)
25. Environment provisioning

---
**Selected References:**

1. **[The Fast Thin‑Client Shuffle with o1](https://natecombs.substack.com/p/the-fast-thin-client-shuffle-with)**

   * **FastAPI [REST](https://en.wikipedia.org/wiki/REST) Backend for Thin Clients**
     Architected a Python FastAPI service exposing `/visualize` and other JSON endpoints, cleanly separating server logic from JavaScript UIs for targeted CI tests of API contracts and payloads.

     * **Keywords:** FastAPI · [REST API](https://en.wikipedia.org/wiki/REST) design · separation of concerns · endpoint testing
   * **CI‑Friendly Project Scaffolding & Modular Layout**
     Organized code into `static/` (JS) and `templates/` (HTML) directories with clear module boundaries, supporting repeatable build‑deploy scaffolding and automated UI/endpoint validation in CI pipelines.

     * **Keywords:** project scaffolding · modular architecture · CI integration · automated UI testing

2. **[Backus‑Naur Form and o3](https://natecombs.substack.com/p/backus-naur-form-granmars-and-o3)**

   * **AI‑Assisted CI Pipeline Debugging**
     Analyzed \~2,000 lines of GitHub Actions logs with chain‑of‑thought LLM prompts (o1, o3‑mini, o3‑mini‑high) to pinpoint and resolve Pyparsing parser failures downstream of PDF generation.

     * **Keywords:** GitHub Actions · CI log analysis · chain‑of‑thought prompts · LLM‑driven debugging · parser error resolution
   * **Parser Robustness & Regression Testing**
     Refactored the core Pyparsing grammar to handle new edge cases—removed obsolete Graphviz code—and integrated automated regression tests into the CI workflow to catch future parsing regressions.

     * **Keywords:** Pyparsing grammar · edge‑case handling · regression tests · CI integration · parser resilience

3. **[AI on EC2 Over Easy, Part I](https://natecombs.substack.com/p/ai-on-ec2-over-easy-part-i)**

   * **Cloud Infrastructure Provisioning & Cost Control**
     Automated spin‑up of `g4dn.xlarge` EC2 instances via AWS Console/CLI for LLM experimentation, selecting GPU‑enabled AMIs (Deep Learning OSS Nvidia Driver) and a “rent‑by‑the‑hour” strategy to minimize expenses.

     * **Keywords:** AWS EC2 (g4dn.xlarge) · AMI selection · GPU‑enabled PyTorch · cost optimization · instance lifecycle
   * **Remote Development Workflow Integration**
     Established secure SSH/SCP transfers from Windows WSL2 to EC2, leveraging Amazon Connect’s web interface and WSL2 console for seamless script deployment and reproducible Python training runs.

     * **Keywords:** SSH/SCP · WSL2 integration · Amazon Connect · reproducible execution · remote debugging

4. **[SonarQube Installation on Windows](https://natecombs.substack.com/p/sonarqube-installation-on-windows)**

   * **Containerized SonarQube on WSL2**
     Deployed SonarQube in Docker with dedicated volumes and an isolated network, enabling fast, scalable CI test environments.

     * **Keywords:** Docker · volumes · network · SonarQube · WSL2
   * **Streamlined QA Pipeline Setup**
     Bootstrapped projects at `localhost:9000`, automated baseline key generation and admin credential rotation, and plugged SonarQube scans into Windows CI workflows.

     * **Keywords:** SonarQube setup · baseline keys · credential rotation · QA pipeline integration

5. **[Ollama and the Laptop](https://natecombs.substack.com/p/ollama-and-the-laptop)**

   * **Reproducible LLM Host Environment**
     Scripted installation of Ollama on Windows WSL2 to run open‑source Llama2 (7B) models locally, providing low‑latency inference and eliminating external API dependencies for testing.

     * **Keywords:** Ollama installation · WSL2 provisioning · Llama2 local host · reproducible environment
   * **IDE‑Integrated DevOps Workflow**
     Integrated VS Code with WSL2/Ollama for interactive prompt testing and rapid iteration of LLM query design, streamlining local development and evaluation.

     * **Keywords:** VS Code WSL2 integration · interactive debugging · prompt engineering · local‑first testing

6. **[Automated CI Workflow Provisioning](https://natecombs.substack.com/p/chatgpt-o1-does-github-actions)**

   * **GitHub Actions for Unit‑Test Automation**
     Defined a pipeline to run Python unit tests on every push/PR: installed dependencies (`requirements.txt`), set up NLTK data, and securely injected the OpenAI API key via GitHub Secrets.

     * **Keywords:** GitHub Actions · unit‑test automation · requirements.txt · NLTK setup · GitHub Secrets
   * **CI Environment Troubleshooting & Optimization**
     Debugged dependency/install failures by adding explicit NLTK downloads, refining `requirements.txt`, and planning caching and matrix testing; integrated style checks (black, flake8, mypy) with continue‑on‑error.

     * **Keywords:** CI troubleshooting · dependency management · caching strategies · matrix testing · style‑check integration

7. **[ChatGPT and a Dialog Pop‑up](https://natecombs.substack.com/p/chatgpt-and-a-dialog-pop-up)**

   * **AI‑Driven UI Integration**
     Used ChatGPT o1‑preview to generate C++ dialog pop‑up code and update Visual Studio resources, then integrated the feature into the CI build pipeline—cutting manual effort.

     * **Keywords:** ChatGPT o1‑preview · AI‑driven code generation · Visual Studio resources · C++ CI integration
   * **Iterative AI‑Assisted Debugging**
     Employed prompt engineering with ChatGPT to pinpoint and fix build/linker errors (resource IDs, GDI+), validating each correction via CI test builds for pipeline reliability.

     * **Keywords:** prompt engineering · iterative debugging · linker error resolution · CI validation

8. **[Prompt Twists and Code Turns with o1](https://natecombs.substack.com/p/prompt-twists-and-code-turns-with)**

   * **Graceful Degradation in Text‑Analysis Services**
     Designed service logic so Redis clients default to `None`, vector‑store calls wrapped in try/except, and embedding caching skipped when needed—keeping CI runs stable.

     * **Keywords:** graceful degradation · exception handling · CI resilience
   * **Improved Observability & Fallback**
     Added logging for Redis connectivity and automatically fell back to direct OpenAI API calls when Redis was unavailable—eliminating external dependency failures.

     * **Keywords:** fallback logic · logging · prompt engineering · dependency isolation

9. **[Automated Architecture Diagram Generation](https://natecombs.substack.com/p/ai-flashlights-and-happy-holiday)**

   * **SysML→Graphviz→LaTeX Pipeline**
     Extended the BSF Manage GitHub Actions pipeline to auto‑generate SysML reports, convert them into Graphviz DOT diagrams and LaTeX architecture docs (with Overleaf rendering), dispatching PNG/PDF artifacts to a management repo.

     * **Keywords:** GitHub Actions · SysML parser · Graphviz DOT · LaTeX report · repository\_dispatch · CI error‑fallback
   * **Test‑Case–Driven Parser Resilience**
     Upgraded the SysML parser in response to new test‑case breakages: used an iterative, LLM‑assisted debugging loop to refine and generalize the grammar, with regression tests in CI to catch edge‑case failures.

     * **Keywords:** test‑case driven development · regression testing · grammar refinement · LLM collaboration

10. **[A Late Night with o1](https://natecombs.substack.com/p/a-late-night-with-o1)**

    * **LLM‑Assisted CI/CD Pipeline Debugging**
      Employed OpenAI o1 and o1‑mini in a GitHub Actions workflow to ingest verbose pipeline logs, craft chain‑of‑thought prompts that pinpointed YAML syntax and dependency errors, and iteratively refine workflow scripts—drastically reducing build failures [1].

      * **Keywords:** CI/CD pipeline debugging · GitHub Actions · LLM‑assisted troubleshooting · prompt engineering
    * **Automated Error‑Handling & Recovery Logic**
      Generated and validated fallback steps (e.g., raw log dumps, retry hooks) via o1‑driven scripts embedded in CI jobs—ensuring resilient builds by automatically catching, diagnosing, and remediating common pipeline failures [1].

      * **Keywords:** automated error handling · fallback logic · CI resiliency · LLM‑driven remediation

11. **[Chatting up o1](https://natecombs.substack.com/p/chatting-up-o1)**

    * **Model Benchmarking for Software Workflows**
      Conducted side‑by‑side evaluations of ChatGPT 4o vs. o1 series on code‑generation and debugging tasks, using detailed context briefs to demonstrate o1’s superior chain‑of‑thought reasoning and accuracy in resolving complex software issues.

      * **Keywords:** LLM benchmarking · chain‑of‑thought models · prompt design · software task evaluation
    * **Context‑Rich Prompt Engineering**
      Transitioned from ad‑hoc prompts to comprehensive “briefs” supplying full code snippets, config files, and test outputs—enabling o1 to generate precise code fixes, test scaffolds, and CI/CD YAML fragments that seamlessly plugged into existing DevOps pipelines [1].

      * **Keywords:** context briefs · prompt engineering · test scaffolding · CI/CD configuration generation

12. **[Towards Automating a GitHub Workflow](https://natecombs.substack.com/p/towards-automating-a-github-workflow)**

    * **Generative‑AI–Powered Diagram Generation**
      Implemented a GitHub Actions pipeline that reads repo source, invokes ChatGPT to produce LaTeX architectural diagrams, and uses `repository_dispatch` to deliver rendered outputs (or raw PDFs on failure) to a management repo.

      * **Keywords:** GitHub Actions · OpenAI API · LaTeX automation · repository\_dispatch · CI error‑fallback
    * **End‑to‑End CI Validation & Reporting**
      Integrated style checks (flake8, black), unit tests, and OpenAI model calls into a single workflow, automating build‑time document generation and versioned artifact commits.

      * **Keywords:** checkout/setup‑python · flake8/black · unit‑tests · automated reporting · CI pipeline orchestration

13. **[Towards Communicating Software Architecture](https://natecombs.substack.com/p/towards-communicating-software-architecture)**

    * **SysML‑Based Architecture Modeling in CI**
      Extended the “Tools” pipeline to generate SysML/DML reports via ChatGPT, then dispatched them to the “Manage” pipeline where a Python converter transforms SysML into Graphviz DOT and renders PNG diagrams automatically.

      * **Keywords:** SysML/DML grammar · ChatGPT prompt‑engineering · generate\_sysml\_report.py · Graphviz automation · cross‑repo dispatch
    * **Robust Multi‑Stage GitHub Actions Orchestration**
      Defined two coordinated Actions workflows—one for code analysis & SysML generation, another for report extraction, Graphviz rendering, README updates, and artifact commit‑push—to ensure end‑to‑end CI/CD traceability [1].

      * **Keywords:** multi‑repo CI · setup‑python/install‑deps · render‑dot/upload‑png · update‑readme · pipeline traceability

14. **[Vector Databases and Knotweed o1](https://natecombs.substack.com/p/vector-databases-and-knotweed-o1)**

    * **Redis Vector DB Integration & Embedding Caching**
      Engineered a prototype pipeline using Redis’s cloud vector database to cache OpenAI embeddings, implementing SHA‑256 hashing of text windows and anchors in Python to dedupe requests and slash API costs in CI runs.

      * **Keywords:** Redis Vector Database · embedding caching · SHA‑256 hashing · deduplication · cost optimization · CI pipeline performance
    * **Generative‑AI Documentation Automation in CI/CD**
      Built an o1‑GPT–driven documentation workflow—parsing commit logs (`git log -p`) and server code—to auto‑generate technical summaries, with plans to embed into GitHub Actions for automated progress reporting [1].

      * **Keywords:** OpenAI o1 model · prompt engineering · CI/CD Actions · automated documentation · commit‑history summarization

15. **[My Late Night Model Context Protocol](https://natecombs.substack.com/p/my-late-night-model-context-protocol-732)**

    * **ASGI‑Based MCP Endpoint Integration**
      Refactored a FastAPI server to mount an [ASGI](https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface) `/mcp` adapter, exposing Model Context Protocol tools for seamless Claude Desktop–backend communication in automated test suites.

      * **Keywords:** ASGI middleware · FastAPI · MCP endpoint · tool mounting · automated testing
    * **CI‑Style Prompt‑Engineering & Resiliency**
      Developed JavaScript visualization templates with built‑in fallback logic for server connectivity failures and incorporated iterative prompt refinements into CI validation loops to ensure pipeline robustness.

      * **Keywords:** prompt engineering · JavaScript template tooling · error handling · CI validation · pipeline resilience

16. **[The Milagro Beanfield War and My Model Context Protocol Road Trip](https://natecombs.substack.com/p/the-milagro-beanfield-war-and-my)**

    * **LLM Client–Server Integration**
      Connected Claude Desktop as the AI front‑end to a Python REST API, resolving serialization and formatting errors to enable reliable client‑server workflows in automated test pipelines.

      * **Keywords:** LLM client integration · REST API · data serialization · automated testing
    * **AI‑Driven JavaScript Endpoints & CI Validation**
      Designed prompt‑engineered CI validation steps—with fallback logic for connectivity failures and iterative prompt refinements—to ensure resilient, consistent pipeline executions.

      * **Keywords:** JavaScript endpoint design · prompt engineering · error handling · CI resiliency

17. **[Python Code Smells within the Generative AI Ecosystem](https://medium.com/ai-advances/python-code-smells-within-the-generative-ai-ecosystem-towards-measuring-llm-coding-insights-with-4bdcff628340)**

    * **Automated SonarQube Integration**
      Integrated SonarQube into Python LLM code‑generation pipelines to detect S905 code smells.

      * **Keywords:** SonarQube · static code analysis · code smell detection · quality gates · CI/CD integration
    * **Reproducible LLM Test Environments**
      Scripted provisioning of reproducible Ollama‐based LLM test environments on WSL2.

      * **Keywords:** Ollama · WSL2 · environment provisioning · dependency automation · reproducible builds

18. **[Amazon Web Services Fine‑Tunes a Large Language Model](https://medium.com/ai-advances/amazon-web-services-fine-tunes-a-large-language-model-using-sagemaker-66b7f14ff8fd)**

    * **Automated SageMaker Fine‑Tuning Pipelines**
      Orchestrated LLM fine‑tuning via AWS SageMaker JumpStart and the SageMaker Python SDK in Jupyter notebooks, integrating model training jobs into CI workflows.

      * **Keywords:** SageMaker JumpStart · Python SDK · Jupyter notebooks · CI integration
    * **Cost‑Governed, Secure Deployment**
      Designed IAM strategies, S3 data pipelines, and AWS Budget Alerts to enforce cost governance and secure resource provisioning in a DevOps environment.

      * **Keywords:** IAM roles · S3 management · AWS CLI automation · Budget Alerts · cost monitoring

19. **[ChatGPT reveals a Riverlands Endurance Run](https://medium.com/ai-advances/chatgpt-reveals-a-riverlands-endurance-run-2d4f9c512dd0)**

    * **Automated Geospatial Data Pipeline**
      Built a GPX ingestion and visualization workflow in ChatGPT‑4o’s Code Interpreter using Python (`gpxpy`, `pandas`, `numpy`) and Matplotlib to generate maps and timelines within CI runs.

      * **Keywords:** GPT‑4o Code Interpreter · gpxpy · pandas · numpy · matplotlib · CI automation
    * **Prompt‑Driven Testing & Dependency Management**
      Orchestrated prompt “hints” to control module usage, implemented iterative error handling, and validated outputs—mirroring a CI feedback loop for AI‑generated code.

      * **Keywords:** prompt engineering · dependency management · error handling · iterative testing · CI feedback loop

20. **[How Many Loops Did I Run? GPT‑4o, GPS Data, and the Art of Asking the Right Question](https://medium.com/ai-advances/how-many-loops-did-i-run-gpt-4o-canvas-gps-data-and-asking-the-right-question-d024667738d8)**

    * **GPT‑4o Canvas in Code‑Gen Workflows**
      Integrated GPT‑4o Canvas into automated code‑generation workflows, using a Python sandbox for rapid prototyping and validation of geospatial algorithms.

      * **Keywords:** GPT‑4o Canvas · code generation · geospatial algorithms · CI testing
    * **Loop‑Counting Algorithm Development**
      Developed and iterated a loop‑counting algorithm with `gpxpy`, `numpy`, and `geopy`, using Matplotlib visualizations to verify accuracy in CI pipelines.

      * **Keywords:** gpxpy · numpy · geopy · Matplotlib · CI automation

21. **[Does Good Software Engineering Improve LLM Performance?](https://medium.com/ai-advances/does-good-software-engineering-improve-the-performance-of-large-language-models-with-software-tasks-e31c0e3626a1)**

    * **REST‑Style Python Services & JS Visualization**
      Architected FastAPI backends paired with JavaScript clients to enable seamless frontend‑backend integration and streamlined containerized deployments.

      * **Keywords:** FastAPI · JS visualization · containerization · backend‑frontend integration
    * **Agile Prototyping & LLM‑Driven Code Review**
      Used Chain‑of‑Thought prompting to refine and iteratively modularize and test code.

      * **Keywords:** agile prototyping · LLM code review · Chain‑of‑Thought prompts · modular testing

22. **[Software Development with ChatGPT o1‑preview: A Brain‑Spans Approach](https://medium.com/ai-advances/software-development-with-chatgpt-o1-preview-a-brain-spans-approach-99d6142d7193)**

    * **C++ GUI Extension & Sentiment Hooks**
      Collaborated with ChatGPT o1‑preview to extend a Visual Studio C++ GUI, adding clipboard/file I/O and sentiment‑analysis hooks with peer‑reviewed config adjustments.

      * **Keywords:** ChatGPT o1‑preview · C++ GUI · Visual Studio · sentiment analysis
    * **Python Backend Optimization**
      Added batching & caching for OpenAI embedding requests, introduced detailed logging, and exposed an HTTP `/visualize` endpoint for automated test reporting.

      * **Keywords:** batching · caching · logging · FastAPI endpoint · CI reporting

23. **[Code Generation with ChatGPT o1‑preview as a Story of Human‑AI Collaboration](https://medium.com/ai-advances/code-generation-with-chatgpt-o1-preview-as-a-story-of-human-ai-collaboration-c80ecd9737ec)**

    * **Iterative Multi‑Prompt Workflow**
      Orchestrated step‑by‑step prompts with ChatGPT to generate Python (NLTK, LangChain) and C++ (ISO C++20) [sentiment‑analysis tools](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Fae8c25cd-5374-4c39-872e-819f74051836_875x412.png), emphasizing testing and cleanup.

      * **Keywords:** iterative prompting · NLTK · LangChain · C++20 · tool generation
    * **Hybrid C++/Python Architecture**
      Integrated a C++ client with a Python REST service for OpenAI embeddings, simplifying dependency management and accelerating CI build times.

      * **Keywords:** hybrid architecture · dependency management · CI build optimization

24. **[Migrating C++ & Python into a Single Visual Studio Solution](https://natecombs.substack.com/p/software-development-with-chatgpt-6d4)**

    * **Unified Multi‑Language Build/Debug Pipeline**
      Consolidated a C++ client and Python server into one Visual Studio solution, streamlining build/debug configurations and reducing DevOps setup overhead.

      * **Keywords:** Visual Studio integration · multi‑language pipeline · IDE configuration · DevOps toolchain
    * **Automated End‑to‑End Integration Tests**
      Added a Python `unittest` project to launch the server, provision environments, validate requests/responses, and tear down via `subprocess`—fully automated in CI.

      * **Keywords:** Python integration tests · CI automation · test environment provisioning · automated teardown

25. **[Refactoring Repos with ChatGPT‑Driven Prompt Engineering](https://natecombs.substack.com/p/software-development-with-chatgpt)**

    * **GitHub Repo Structure Refactor**
      Used ChatGPT to generate and execute `git mv` and directory‑creation commands, reorganizing source, configs, and tests into a CI‑friendly layout.

      * **Keywords:** git automation · repository refactoring · prompt engineering · CI‑ready structure
    * **Reproducible “Test” Branch Workflow**
      Instituted a scripted `.gitkeep` strategy for empty directories and staged commits—ensuring version‑controlled scaffolding and maintainable project topology.

      * **Keywords:** branch management · directory scaffolding · .gitkeep · maintainability

---
**Footnotes:**

[1] In the articles and posts referenced above, I use the term CI/CD pipelines—such as those in GitLab—interchangeably with GitHub Actions workflows. While GitLab CI/CD and GitHub Actions differ in implementation and features, the term 'CI/CD' is used here in a general sense to refer to automation systems that support continuous integration and delivery. I work with both GitLab and GitHub, though only GitHub is cited in this context.[GitLab CI/CD versus GitHub Actions](https://graphite.dev/guides/gitlab-cicd--vs-github-actions).

---

For the complete archive of technical posts:

📘 [Substack Articles](https://natecombs.substack.com/)

📘 [Medium Writings](https://medium.com/me/stories/public)


