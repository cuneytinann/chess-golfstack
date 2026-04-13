# golfchess

A fully functional chess game in a single HTML file — **3260 bytes**.

## Features

- All standard pieces with correct movement rules
- Castling (kingside and queenside)
- En passant
- Pawn promotion (choose Q, R, B, or N)
- Check detection — board locks when no legal moves remain
- 50-move rule draw
- Checkmate and stalemate detection

## Design goals

- No UI chrome. No labels, no highlights, no move indicators.
- No external dependencies.
- No build step. Open in browser and play.
- All variable and function names are 1–2 characters.
- Castle rights stored as a 4-bit integer.
- Board stored as a 64-character string array. Uppercase = white, lowercase = black, dot = empty.

## How to play

Open `golfchess.html` in any browser. White moves first (uppercase letters). Click a piece, then click its destination. Pawn promotion shows a letter picker. When the game ends the board freezes. Refresh to restart.

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

Tek bir HTML dosyasında tam işlevsel bir satranç oyunu — **3260 byte**.

## Özellikler

- Tüm standart taşlar ve doğru hareket kuralları
- Rok (kısa ve uzun)
- En passant
- Piyon terfisi (Q, R, B veya N seçimi)
- Şah kontrolü — legal hamle kalmayınca tahta kilitlenir
- 50 hamle kuralı beraberliği
- Mat ve pat tespiti

## Tasarım hedefleri

- Arayüz yok. Etiket, renk, hamle göstergesi yok.
- Harici bağımlılık yok.
- Build adımı yok. Tarayıcıda açıp oyna.
- Tüm değişken ve fonksiyon isimleri 1–2 karakter.
- Rok hakları 4 bitlik tam sayıda saklanır.
- Tahta 64 karakterlik string dizisi. Büyük harf = beyaz, küçük harf = siyah, nokta = boş.

## Nasıl oynanır

`golfchess.html` dosyasını herhangi bir tarayıcıda aç. Beyaz önce oynar (büyük harfler). Bir taşa tıkla, sonra hedef kareye tıkla. Piyon terfisinde harf seçici çıkar. Oyun bitince tahta donar. Yeniden başlamak için sayfayı yenile.

## Taş kodlaması

| Harf | Taş |
|------|-----|
| K / k | Şah |
| Q / q | Vezir |
| R / r | Kale |
| B / b | Fil |
| N / n | At |
| P / p | Piyon |
