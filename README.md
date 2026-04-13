# golfchess

A fully functional two-player chess game in three versions — **8595 bytes total, 219 lines**.

Both sides are played by humans. No AI. No dependencies. No build step.

---

## Versions

### golfchess.html — click to play
**3054 bytes · 79 lines**

Open in a browser and play by clicking. Click a piece, then click its destination. The most playable version — no typing required, works on any device including mobile.

### golfchess-prompt.html — prompt to play
**2689 bytes · 70 lines**

The shortest version. Open in a browser; a prompt dialog shows the board as 8 rows of letters and waits for input. Type a move in algebraic notation (e.g. `e2e4`) and press OK. Less comfortable to play but the leanest code.

### golfchess.js — terminal
**2852 bytes · 70 lines**

Run with `node golfchess.js`. The board prints to the terminal with coordinates, the current side is shown, and you type moves the same way. Requires Node.js. Best terminal experience.

---

## Comparison

| | golfchess.html | golfchess-prompt.html | golfchess.js |
|---|---|---|---|
| Size | 3054 bytes | 2689 bytes | 2852 bytes |
| Lines | 79 | 70 | 70 |
| Interface | Click | prompt() | Terminal |
| Requires | Browser | Browser | Node.js |
| Playability | ★★★ | ★☆☆ | ★★☆ |
| Code size | ★★☆ | ★★★ | ★★☆ |

---

## How to move

All three versions use the same algebraic notation: **source square + destination square**.

```
e2e4   move pawn from e2 to e4
g1f3   move knight from g1 to f3
e1g1   castle kingside (king moves two squares)
e1c1   castle queenside
```

Columns are `a–h` (left to right), rows are `1–8` (bottom to top from white's perspective).

Pawn promotion: when a pawn reaches the last rank, you choose the piece. In the click version a picker appears. In prompt and node versions a second prompt/input asks for `Q`, `R`, `B`, or `N`.

---

## Piece encoding

| Letter | Piece |
|--------|-------|
| K / k | King |
| Q / q | Queen |
| R / r | Rook |
| B / b | Bishop |
| N / n | Knight |
| P / p | Pawn |

Uppercase = white, lowercase = black.

---

## Rules

Compliant with FIDE rules. The only missing element is a clock — there is no time control.

There is no checkmate or stalemate announcement. When a side has no legal moves, the board simply freezes (click version) or stops accepting input. The players will know.

The 50-move rule is implemented. This also covers the two other draw conditions in practice: insufficient material (if neither side can force mate in 50 moves, the rule triggers) and threefold repetition (if both players keep repeating moves, no pawn move or capture occurs and the counter eventually reaches 50). These are not tracked explicitly — the 50-move rule absorbs them.

---
---

# golfchess

Üç versiyonda tam işlevsel iki kişilik satranç — **toplam 8595 byte, 219 satır**.

Her iki tarafı da insan oynar. Yapay zeka yok. Bağımlılık yok. Build adımı yok.

---

## Versiyonlar

### golfchess.html — tıklamalı
**3054 byte · 79 satır**

Tarayıcıda aç, tıklayarak oyna. Bir taşa tıkla, hedef kareye tıkla. En oynanabilir versiyon — yazı yazmak gerekmez, mobil dahil her cihazda çalışır.

### golfchess-prompt.html — prompt ile
**2689 byte · 70 satır**

En kısa versiyon. Tarayıcıda aç; bir prompt penceresi tahtayı 8 satır harf olarak gösterir ve girdi bekler. Hamleyi algebraik notasyonla yaz (örn. `e2e4`) ve Tamam'a bas. Oynaması daha az konforlu ama en sade kod.

### golfchess.js — terminal
**2852 byte · 70 satır**

`node golfchess.js` ile çalıştır. Tahta koordinatlarıyla terminale yazdırılır, sıradaki taraf gösterilir, hamleleri aynı şekilde yazarsın. Node.js gerektirir. En iyi terminal deneyimi.

---

## Karşılaştırma

| | golfchess.html | golfchess-prompt.html | golfchess.js |
|---|---|---|---|
| Boyut | 3054 byte | 2689 byte | 2852 byte |
| Satır | 79 | 70 | 70 |
| Arayüz | Tıklama | prompt() | Terminal |
| Gereksinim | Tarayıcı | Tarayıcı | Node.js |
| Oynanabilirlik | ★★★ | ★☆☆ | ★★☆ |
| Kod boyutu | ★★☆ | ★★★ | ★★☆ |

---

## Hamle nasıl yapılır

Üç versiyon da aynı notasyonu kullanır: **kaynak kare + hedef kare**.

```
e2e4   piyonu e2'den e4'e taşı
g1f3   atı g1'den f3'e taşı
e1g1   kısa rok (şah iki kare kayar)
e1c1   uzun rok
```

Sütunlar `a–h` (soldan sağa), sıralar `1–8` (beyazın perspektifinden aşağıdan yukarıya).

Piyon terfisi: piyon son sıraya ulaşınca taş seçimi yapılır. Tıklamalı versiyonda seçici çıkar. Prompt ve node versiyonlarında ikinci bir prompt/girdi `Q`, `R`, `B` veya `N` sorar.

---

## Taş kodlaması

| Harf | Taş |
|------|-----|
| K / k | Şah |
| Q / q | Vezir |
| R / r | Kale |
| B / b | Fil |
| N / n | At |
| P / p | Piyon |

Büyük harf = beyaz, küçük harf = siyah.

---

## Kurallar

FIDE kurallarıyla uyumludur. Eksik olan tek şey saattir — süre kontrolü yoktur.

Mat veya pat bildirimi yoktur. Bir tarafın legal hamlesi kalmayınca tahta donar (tıklamalı versiyon) veya girdi kabul etmeyi bırakır. Oyuncular zaten anlayacaktır.

50 hamle kuralı uygulanmaktadır. Bu kural pratikte diğer iki beraberlik koşulunu da kapsar: yetersiz malzeme (hiçbir taraf 50 hamlede mat edemiyorsa kural devreye girer) ve üçlü tekrar (oyuncular aynı hamleleri tekrar ederse piyon hamlesi veya yeme olmadığından sayaç sonunda 50'ye ulaşır). Bu durumlar ayrıca takip edilmez — 50 hamle kuralı onları kapsar.
