# golfchess

A fully functional two-player chess game in a single HTML file. Both sides are played by humans. No AI.

**3054 bytes. 79 lines.**

## Rules

Compliant with FIDE rules. The only missing element is a clock — there is no time control.

The 50-move rule is implemented. This also covers the two other draw conditions in practice: insufficient material (if neither side can mate in 50 moves, the rule triggers) and threefold repetition (if both players keep repeating moves, the 50-move counter never resets and the game eventually draws). These cases are not tracked explicitly — the 50-move rule absorbs them.

There is no checkmate or stalemate announcement. When a side has no legal moves, the board simply freezes. The players will know.

## How to play

Open `golfchess.html` in any browser. White moves first (uppercase letters). Click a piece, then click its destination. Pawn promotion shows a letter picker. Refresh to restart.

## Piece encoding

| Letter | Piece |
|--------|-------|
| K / k | King |
| Q / q | Queen |
| R / r | Rook |
| B / b | Bishop |
| N / n | Knight |
| P / p | Pawn |

---

# golfchess

Tek bir HTML dosyasında tam işlevsel iki kişilik satranç oyunu. Her iki tarafı da insan oynar. Yapay zeka yoktur.

**3054 byte. 79 satır.**

## Kurallar

FIDE kurallarıyla uyumludur. Eksik olan tek şey saattir — süre kontrolü yoktur.

50 hamle kuralı uygulanmaktadır. Bu kural pratikte diğer iki beraberlik koşulunu da kapsar: yetersiz malzeme (hiçbir taraf 50 hamlede mat edemiyorsa kural devreye girer) ve üçlü tekrar (oyuncular aynı pozisyonu tekrar ederse piyon hamlesi veya yeme olmadığından 50 hamle sayacı hiç sıfırlanmaz ve oyun beraberlikle biter). Bu durumlar ayrıca takip edilmez — 50 hamle kuralı onları kapsar.

Mat veya pat bildirimi yoktur. Bir tarafın legal hamlesi kalmayınca tahta donar. Oyuncular zaten anlayacaktır.

## Nasıl oynanır

`golfchess.html` dosyasını herhangi bir tarayıcıda aç. Beyaz önce oynar (büyük harfler). Bir taşa tıkla, sonra hedef kareye tıkla. Piyon terfisinde harf seçici çıkar. Yeniden başlamak için sayfayı yenile.

## Taş kodlaması

| Harf | Taş |
|------|-----|
| K / k | Şah |
| Q / q | Vezir |
| R / r | Kale |
| B / b | Fil |
| N / n | At |
| P / p | Piyon |
