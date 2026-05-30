# BINGO-LSST-CrossCorrelation-JCAP2025
A harmonic space pipeline for detecting the 21 cm HI intensity mapping signal through cross-correlation between BINGO and LSST log-normal mock maps.

├── README.md              # Instruções de instalação, dependências e benchmarks de hardware
├── requisitos.txt         # Versões exatas dos pacotes (healpy, NaMaster, UCLCl, FLASK, etc.)
├── configuracoes/         # Arquivos .ini ou .yaml com os parâmetros fiduciais usados
├── scripts/               # Códigos em Python puro (.py) executados no cluster HPC
│   ├── 01_rodar_flask.py  # Pipeline de geração dos mapas log-normais
│   ├── 02_gnilc_clean.py  # Filtros de separação de componentes
│   └── 03_debiasing.py    # Rotinas de correção aditiva e multiplicativa
└── notebooks/             # Jupyter Notebooks para visualização e análise
    ├── matriz_covariancia.ipynb # Plot da matriz solicitado pelo Prof. Rogério
    └── gerar_figuras_jcap.ipynb # Geração dos gráficos de SNR e b² do artigo
