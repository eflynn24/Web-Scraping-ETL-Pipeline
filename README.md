**Project: Web Scraping & LLM Data Pipeline**

Build an ETL pipeline that collects website data, processes and cleans the text, applies quality filtering, and prepares a dataset suitable for large language model (LLM) training and evaluation.

**Project Objectives**

Query Common Crawl data

Extract web page content

Clean and normalize text

Filter low-quality content

Score documents using quality metrics

Create a structured dataset for LLM use

Analyze the resulting dataset

Data quality assessment

<div align="center">

<svg width="100%" viewBox="0 0 1100 430" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="header" x1="0" x2="1">
      <stop offset="0%" stop-color="#24292f"/>
      <stop offset="100%" stop-color="#0969da"/>
    </linearGradient>

    <filter id="shadow" x="-20%" y="-20%" width="140%" height="140%">
      <feDropShadow dx="0" dy="4" stdDeviation="5" flood-opacity="0.15"/>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="1100" height="430" rx="18" fill="#f6f8fa"/>

  <!-- Header -->
  <rect x="0" y="0" width="1100" height="82" rx="18" fill="url(#header)"/>
  <rect x="0" y="55" width="1100" height="27" fill="url(#header)"/>

  <text x="550" y="37"
        text-anchor="middle"
        font-family="Arial, Helvetica, sans-serif"
        font-size="25"
        font-weight="700"
        fill="white">
    Web Scraping &amp; LLM Data Pipeline
  </text>

  <text x="550" y="62"
        text-anchor="middle"
        font-family="Arial, Helvetica, sans-serif"
        font-size="13"
        fill="#dbeafe">
    From raw web data to quality-controlled datasets for LLM applications
  </text>

  <!-- Stage 1 -->
  <g filter="url(#shadow)">
    <rect x="35" y="125" width="135" height="155" rx="12" fill="white" stroke="#d0d7de"/>
    <circle cx="102" cy="157" r="22" fill="#0969da"/>
    <text x="102" y="164" text-anchor="middle"
          font-family="Arial" font-size="21" font-weight="700" fill="white">1</text>

    <text x="102" y="198" text-anchor="middle"
          font-family="Arial" font-size="15" font-weight="700" fill="#24292f">
      Common Crawl
    </text>

    <text x="102" y="222" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      Query web-scale
    </text>
    <text x="102" y="239" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      crawl archives
    </text>

    <rect x="58" y="250" width="89" height="20" rx="10" fill="#ddf4ff"/>
    <text x="102" y="264" text-anchor="middle"
          font-family="Arial" font-size="10" font-weight="600" fill="#0969da">
      WARC / Index
    </text>
  </g>

  <!-- Arrow -->
  <path d="M175 202 L205 202" stroke="#8c959f" stroke-width="3"/>
  <polygon points="205,202 196,196 196,208" fill="#8c959f"/>

  <!-- Stage 2 -->
  <g filter="url(#shadow)">
    <rect x="210" y="125" width="135" height="155" rx="12" fill="white" stroke="#d0d7de"/>
    <circle cx="277" cy="157" r="22" fill="#0969da"/>
    <text x="277" y="164" text-anchor="middle"
          font-family="Arial" font-size="21" font-weight="700" fill="white">2</text>

    <text x="277" y="198" text-anchor="middle"
          font-family="Arial" font-size="15" font-weight="700" fill="#24292f">
      Extraction
    </text>

    <text x="277" y="222" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      Parse HTML
    </text>
    <text x="277" y="239" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      &amp; extract content
    </text>

    <rect x="233" y="250" width="89" height="20" rx="10" fill="#ddf4ff"/>
    <text x="277" y="264" text-anchor="middle"
          font-family="Arial" font-size="10" font-weight="600" fill="#0969da">
      Raw Text
    </text>
  </g>

  <!-- Arrow -->
  <path d="M350 202 L380 202" stroke="#8c959f" stroke-width="3"/>
  <polygon points="380,202 371,196 371,208" fill="#8c959f"/>

  <!-- Stage 3 -->
  <g filter="url(#shadow)">
    <rect x="385" y="125" width="135" height="155" rx="12" fill="white" stroke="#d0d7de"/>
    <circle cx="452" cy="157" r="22" fill="#8250df"/>
    <text x="452" y="164" text-anchor="middle"
          font-family="Arial" font-size="21" font-weight="700" fill="white">3</text>

    <text x="452" y="198" text-anchor="middle"
          font-family="Arial" font-size="15" font-weight="700" fill="#24292f">
      Clean &amp; Normalize
    </text>

    <text x="452" y="222" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      Remove noise
    </text>
    <text x="452" y="239" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      normalize text
    </text>

    <rect x="408" y="250" width="89" height="20" rx="10" fill="#fbefff"/>
    <text x="452" y="264" text-anchor="middle"
          font-family="Arial" font-size="10" font-weight="600" fill="#8250df">
      Clean Text
    </text>
  </g>

  <!-- Arrow -->
  <path d="M525 202 L555 202" stroke="#8c959f" stroke-width="3"/>
  <polygon points="555,202 546,196 546,208" fill="#8c959f"/>

  <!-- Stage 4 -->
  <g filter="url(#shadow)">
    <rect x="560" y="125" width="135" height="155" rx="12" fill="white" stroke="#d0d7de"/>
    <circle cx="627" cy="157" r="22" fill="#bf8700"/>
    <text x="627" y="164" text-anchor="middle"
          font-family="Arial" font-size="21" font-weight="700" fill="white">4</text>

    <text x="627" y="198" text-anchor="middle"
          font-family="Arial" font-size="15" font-weight="700" fill="#24292f">
      Quality Filter
    </text>

    <text x="627" y="222" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      Deduplicate
    </text>
    <text x="627" y="239" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      filter low-quality data
    </text>

    <rect x="583" y="250" width="89" height="20" rx="10" fill="#fff8c5"/>
    <text x="627" y="264" text-anchor="middle"
          font-family="Arial" font-size="10" font-weight="600" fill="#9a6700">
      Valid Records
    </text>
  </g>

  <!-- Arrow -->
  <path d="M700 202 L730 202" stroke="#8c959f" stroke-width="3"/>
  <polygon points="730,202 721,196 721,208" fill="#8c959f"/>

  <!-- Stage 5 -->
  <g filter="url(#shadow)">
    <rect x="735" y="125" width="135" height="155" rx="12" fill="white" stroke="#d0d7de"/>
    <circle cx="802" cy="157" r="22" fill="#1a7f37"/>
    <text x="802" y="164" text-anchor="middle"
          font-family="Arial" font-size="21" font-weight="700" fill="white">5</text>

    <text x="802" y="198" text-anchor="middle"
          font-family="Arial" font-size="15" font-weight="700" fill="#24292f">
      Quality Scoring
    </text>

    <text x="802" y="222" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      Score documents
    </text>
    <text x="802" y="239" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      using quality metrics
    </text>

    <rect x="758" y="250" width="89" height="20" rx="10" fill="#dafbe1"/>
    <text x="802" y="264" text-anchor="middle"
          font-family="Arial" font-size="10" font-weight="600" fill="#1a7f37">
      Scored Data
    </text>
  </g>

  <!-- Arrow -->
  <path d="M875 202 L905 202" stroke="#8c959f" stroke-width="3"/>
  <polygon points="905,202 896,196 896,208" fill="#8c959f"/>

  <!-- Stage 6 -->
  <g filter="url(#shadow)">
    <rect x="910" y="125" width="155" height="155" rx="12" fill="white" stroke="#d0d7de"/>
    <circle cx="987" cy="157" r="22" fill="#cf222e"/>
    <text x="987" y="164" text-anchor="middle"
          font-family="Arial" font-size="21" font-weight="700" fill="white">6</text>

    <text x="987" y="198" text-anchor="middle"
          font-family="Arial" font-size="15" font-weight="700" fill="#24292f">
      Dataset &amp; Analysis
    </text>

    <text x="987" y="222" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      Structured LLM
    </text>
    <text x="987" y="239" text-anchor="middle"
          font-family="Arial" font-size="11" fill="#57606a">
      dataset + statistics
    </text>

    <rect x="944" y="250" width="86" height="20" rx="10" fill="#ffebe9"/>
    <text x="987" y="264" text-anchor="middle"
          font-family="Arial" font-size="10" font-weight="600" fill="#cf222e">
      JSON / Parquet
    </text>
  </g>

  <!-- Bottom metrics -->
  <text x="550" y="322"
        text-anchor="middle"
        font-family="Arial, Helvetica, sans-serif"
        font-size="14"
        font-weight="700"
        fill="#24292f">
    Data Quality Assessment
  </text>

  <g font-family="Arial, Helvetica, sans-serif" font-size="11" fill="#57606a">
    <rect x="135" y="345" width="145" height="38" rx="19" fill="white" stroke="#d0d7de"/>
    <text x="207" y="369" text-anchor="middle">Completeness</text>

    <rect x="295" y="345" width="145" height="38" rx="19" fill="white" stroke="#d0d7de"/>
    <text x="367" y="369" text-anchor="middle">Duplicate Rate</text>

    <rect x="455" y="345" width="145" height="38" rx="19" fill="white" stroke="#d0d7de"/>
    <text x="527" y="369" text-anchor="middle">Text Quality</text>

    <rect x="615" y="345" width="145" height="38" rx="19" fill="white" stroke="#d0d7de"/>
    <text x="687" y="369" text-anchor="middle">Length Distribution</text>

    <rect x="775" y="345" width="145" height="38" rx="19" fill="white" stroke="#d0d7de"/>
    <text x="847" y="369" text-anchor="middle">Language / Metadata</text>
  </g>

  <text x="550" y="410"
        text-anchor="middle"
        font-family="Arial, Helvetica, sans-serif"
        font-size="11"
        fill="#8c959f">
    ETL • Web Data Processing • Quality Control • LLM Dataset Preparation • Data Analysis
  </text>
</svg>

</div>
