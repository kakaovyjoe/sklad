SKLADOVÝ SYSTÉM – ZDROJOVÝ PROJEKT PRO ANDROID

Projekt převádí základní logiku Excelu skladovy_system_tablet.xlsx do jednoduché aplikace pro Android.
Obsahuje položky načtené z listu Data (EAN + název), skladové oddíly Kaucuk a Chemie, přičítání krabic/kusů, ruční množství, součty a export CSV.

DŮLEŽITÉ
- Toto je zdrojový projekt, nikoli již zkompilovaný APK soubor.
- Počty se ukládají do lokálního úložiště aplikace na daném zařízení. Nejsou automaticky synchronizovány s jiným mobilem/tabletem.
- Před použitím v reálném skladu otestujte chování a udělejte export CSV jako zálohu.

JAK ZÍSKAT APK BEZ ANDROID STUDIA (CLOUDOVÉ SESTAVENÍ)
1. Pokud pracovní PC dovoluje nahrávat soubory na GitHub, přihlas se nebo si vytvoř účet na github.com.
2. Vytvoř nový soukromý repozitář (New repository; Private).
3. Rozbal tento ZIP do složky. Na GitHubu v novém repozitáři zvol Add file > Upload files a nahraj obsah složky projektu včetně skryté složky .github/workflows.
   Pozor: pro upload přes web může být pohodlnější rozbalit ZIP a nahrát soubory po částech; GitHub web nepodporuje nahrání celého adresáře jako adresáře ve všech situacích.
4. Po nahrání otevři záložku Actions. Workflow „Build Android APK“ by se měl spustit automaticky. Pokud ne, otevři jej a zvol Run workflow.
5. Po dokončení otevři výsledek běhu a v sekci Artifacts stáhni „skladovy-system-apk“ (ZIP). Uvnitř je app-debug.apk.
6. Přenes APK do Android tabletu, otevři jej a potvrď instalaci, pokud Android požádá o povolení instalace z daného zdroje.

Pokud GitHub nebo nahrávání souborů blokují pravidla pracovního PC, neobcházej firemní omezení. Zkus domácí počítač nebo požádej IT o schválený postup.

TEST UI BEZ ANDROIDU
Otevři app/src/main/assets/index.html v moderním prohlížeči. Některé prohlížeče při otevírání lokálního HTML blokují načtení products.json; v tom případě je lepší náhled přes lokální server.
