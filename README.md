# Sigil

Prywatny komunikator dla zamkniętej grupy znajomych — czat, rozmowy głosowe z push-to-talk,
udostępnianie ekranu w pełnej jakości, wspólne oglądanie YouTube (watch party) i muzyka w tle.
Bez serwerów i bez abonamentu: wszystko szyfrowane end-to-end i przesyłane bezpośrednio między waszymi komputerami.

To repozytorium zawiera **wyłącznie gotowe instalatory**.

## ⬇️ Pobieranie

👉 **[Najnowsza wersja](https://github.com/mariuszraszei/sigil-releases/releases/latest)** — rozwiń sekcję **Assets** i pobierz plik dla swojego systemu:

| System | Plik |
| --- | --- |
| Windows 10 / 11 | `Sigil-Setup-x.y.z.exe` |
| macOS — Apple M1, M2, M3, M4… | `Sigil-x.y.z-arm64.dmg` |
| macOS — starsze Maki z procesorem Intel | `Sigil-x.y.z-x64.dmg` |

> Nie wiesz, jaki masz procesor w Macu? Menu  → **Ten Mac** → linia „Układ” (Apple M…) albo „Procesor” (Intel…).

---

## 🪟 Instalacja na Windows

1. Uruchom pobrany `Sigil-Setup-….exe`.
2. Windows może pokazać okno **„System Windows ochronił komputer”** — to normalne dla aplikacji bez płatnego certyfikatu.
   Kliknij **Więcej informacji** → **Uruchom mimo to**.
3. Sigil zainstaluje się i uruchomi sam (skrót pojawi się na pulpicie i w menu Start).

**Aktualizacje** przychodzą same — bez serwerów: nowa wersja rozchodzi się P2P między członkami waszych grup, a Sigil instaluje ją dopiero po sprawdzeniu podpisu wydawcy. Gdy będzie gotowa, zobaczysz „Uruchom ponownie”.

---

## 🍎 Instalacja na macOS

1. Otwórz pobrany plik `.dmg`.
2. Przeciągnij ikonę **Sigil** do folderu **Aplikacje** (Applications).
3. Otwórz **Aplikacje** i uruchom **Sigil**. macOS zablokuje go za pierwszym razem, bo aplikacja nie ma płatnego podpisu Apple:
   - kliknij **Gotowe** (albo **OK**),
   - otwórz **Ustawienia systemowe** → **Prywatność i ochrona**,
   - przewiń na dół — przy komunikacie o Sigil kliknij **Otwórz mimo to** → potwierdź hasłem lub Touch ID,
   - uruchom Sigil jeszcze raz i kliknij **Otwórz**.
4. Jeśli macOS twierdzi, że aplikacja jest **„uszkodzona”** i nie da się jej otworzyć:
   otwórz **Terminal** (Cmd + Spacja → wpisz „Terminal”), wklej poniższą linijkę i naciśnij Enter:

   ```bash
   xattr -cr /Applications/Sigil.app
   ```

   Potem uruchom Sigil normalnie.

### Zgody, o które zapyta macOS

| Zgoda | Do czego | Gdzie ją zmienić |
| --- | --- | --- |
| **Mikrofon** | rozmowy głosowe | Ustawienia systemowe → Prywatność i ochrona → Mikrofon |
| **Nagrywanie ekranu** | udostępnianie ekranu (po włączeniu uruchom Sigil ponownie) | … → Nagrywanie ekranu i dźwięku z systemu |
| **Dostępność** | push-to-talk działający w grach i innych aplikacjach | … → Dostępność |

### Różnice na Macu

- Przy udostępnianiu ekranu nie da się przesłać **dźwięku systemu** (ograniczenie macOS) — obraz działa normalnie.
- Aktualizacje Sigil pobiera sam od znajomych (P2P, z weryfikacją podpisu), ale na Macu instalację trzeba potwierdzić: kliknij **Zainstaluj**, otworzy się nowy `.dmg` — przeciągnij Sigil do Aplikacji i zastąp starą wersję. Konto, grupy i wiadomości zostają.

---

## 👋 Pierwsze kroki

1. Po uruchomieniu wpisz swój nick.
2. Poproś znajomego o **kod zaproszenia** (u niego: nazwa grupy u góry → *Zaproś znajomych*).
3. Kliknij **Stwórz lub dołącz** → **Dołącz** i wklej kod.

🔒 Kod zaproszenia to klucz do grupy — przesyłaj go tylko zaufanym osobom.
