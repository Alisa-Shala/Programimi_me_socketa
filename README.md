
# README - Programi i Serverit dhe Klientit

Ky program mundëson krijimin e një sistemi të thjeshtë komunikimi mes klientit dhe serverit duke përdorur soket. Serveri pret lidhje nga klientët dhe proceson komanda si "read", "write", "execute" dhe "sudo" për përmirësimin e të drejtave të përdoruesit. Klienti mund të ndërveprojë me serverin bazuar në llojin e aksesit të dhënë (vetëm për lexim ose qasje e plotë).

## Si të Përdorni Programin:

### 1. **Përgatitja e Mjedisit Virtual:**

#### Përdorimi në Windows (Mjedisi Virtual `venvw`):

- **Hapi 1: Aktivizoni Mjedisin Virtual:**
  Pasi të keni shkarkuar dhe vendosur skriptet në dosjen përkatëse, hapni një dritare të komandës (Command Prompt) dhe kaloni në dosjen ku ndodhen mjediset virtuale:


  cd rruga/deri/tek/dosja/venvw
 

  Aktivizoni mjedisin virtual me komandën:

 
  venvw\Scripts\activate
 

  Pasi ta aktivizoni mjedisin virtual, do të shihni që emri i mjedisit virtual shfaqet në fillim të komandës.

#### Përdorimi në Linux (Mjedisi Virtual `rrjeta`):

- **Hapi 1: Aktivizoni Mjedisin Virtual:**
  Pasi të keni shkarkuar dhe vendosur skriptet në dosjen përkatëse, hapni një terminal dhe kaloni në dosjen ku ndodhen mjediset virtuale:


  cd rruga/deri/tek/dosja/rrjeta


  Aktivizoni mjedisin virtual me komandën:


  source rrjeta/bin/activate


  Pasi të aktivizohet mjedisi virtual, do të shihni emrin e mjedisit në fillim të komandës.

### 2. **Startoni Serverin dhe Klientin:**

- **Hapi 1: Startoni Serverin:**
  Pas aktivizimit të mjedisit virtual, hapni një dritare të komandës (Windows) ose terminal (Linux) dhe startoni serverin duke përdorur komandën:

 
  python server.py


- **Hapi 2: Startoni Klientin:**
  Në një dritare tjetër të komandës (Windows) ose terminal (Linux), startoni klientin me komandën:


  python client.py
 

  Klienti do të lidhet me serverin dhe mund të filloni të dërgoni komanda nga klienti te serveri.

---

### Komandat që mund të përdorni:

- **read:** Kthen të dhënat nga skedari i serverit.
- **write `<new_data>`:** Shtoni të dhëna të reja në skedarin e serverit (duhet të keni qasje të plotë).
- **execute `<command>`:** Ekzekuton komanda në server (duhet të keni qasje të plotë).
- **sudo `<password>`:** Për të bërë upgrade në qasje të plotë (duhet të futni fjalëkalimin e saktë).
- **unsudo:** Për të u kthyer në qasje vetëm për të lexuar.
- **exit:** Përdoret për të dalë nga klienti.


### Përfundim:

Duke përdorur mjediset virtuale, mund të menaxhoni më mirë varësitë dhe të siguroheni që çdo mjedis të ketë versionet përkatëse të bibliotekave të nevojshme për projektin. Aktivizimi dhe përdorimi i mjediseve virtuale është një mënyrë efikase për të mbajtur projektet të izoluara dhe të menaxhueshme.
