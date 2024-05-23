## Instala Python no setup enviromentu

Estabelese Python no konfigura environment iha Windows, Linux, no macOS relativamente simples. Iha ne'e matadalan jerál konaba instala no konfigura python kada plataforma:

### Windows:

1. **Download Python:**
    - Ba Pajina [official Python website](https://www.python.org/).
    - Klik iha tab "Downloads"
    - Download verzaun ikus python ba Windows

2. **Instala Python:**
    - Instala python ne'ebé ita download ona
    - Marka vistu iha lista "Add Python to PATH" durante prosesu instalasaun
    - Halo tuir instalasaun sira no python sei instala iha ita-boot sira nia sistema operasaun Windows nian

3. **Verifika instalasaun:**
    - Ketík `python --version` ka `python3 --version` hodi verifika katak python instala ona no cek nia verzaun

###  Linux:

1. **Instala uza Jestaun pakote(apt ba ubuntu/Debian):**
    - Loke terminal ubuntu linux nian
    - Update lista pakote: `sudo apt update`
    - Instala Python: `sudo apt install python3` 

2. **Verifika Instalasaun**:
    - Ketik `python3 --version` iha terminal no verifika katak python instala ona no cek nia verzaun

### macOS:

1. **Rekomendasaun Instala uza Homebrew:**
    - Instala Homebrew karik ita seidauk iha. Vizita [Homebrew's official website](https://brew.sh/) hodi hare instrusaun konaba instalasaun python ba MacOs
    - Bainhira instala tiha ona Homebrew, tuir mai loke ona Terminal
    - Ketik `brew install python` hodi instala python3
   
2. **Verifika instalasaun:**
    - Ketik `python3 --version` iha terminal no verifika katak python instala ona no cek nia verzaun.
     

### Estabelese virtual Environment (Opsional maibé Rekomenda):

1. **Instala Virtualenv:**
    - Loke terminal (ka Command Prompt iha Windows)
    - Ketik  `pip install virtualenv` hodi instala virtualenv
   
2. **Kria Virtual Environment:**
    - Muda ba folder ne'ebé ita hakarak kria environment
    - Ketik `virtualenv myenv` hodi kria virtual environment fó naran "myenv"
   
3.  **Ativa Virtual environment:**
    - Iha Windows, ketik  ``myenv\Scripts\activate``
    - Iha Linux/macOs, ketik ``source myenv/bin/activate``