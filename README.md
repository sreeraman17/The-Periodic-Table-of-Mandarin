# The Periodic Table of Mandarin (元素周期表 yuánsù zhōuqī biǎo)

An interactive periodic table for learning Mandarin by **parts, not rote lists**. Every word is split into its building blocks, because Chinese runs on roughly 400 syllables that recombine forever: a computer is an electric brain (电脑 diànnǎo), a train is a fire vehicle (火车 huǒchē), a roller coaster is a pass-mountain-car (过山车 guòshānchē). Learn the parts once, recognize words forever.

Built from a personal lesson corpus (Nov 2024 to Jul 2026, HSK 1 and 2): **505 words, 553 parts**.

## Use it

No install, no build, no dependencies. Open `mandarin-periodic-table.html` in any browser, or serve it with GitHub Pages.

## What's inside

- **The Parts.** A grid of building blocks sorted by how many words each one builds (the small number on every tile). Tap a part to see every word it forms.
- **The Words.** The full corpus. Tap any word to see its equation, e.g. 学校 xuéxiào = 学 xué (study) + 校 xiào (school).
- **Search.** Works with tone marks (xuéxiào), tone numbers (xue2xiao4), v for ü (nv3), English, or Hanzi.
- **Same Sound, Different Parts.** Auto-generated cards for overloaded syllables like shi and ji, each meaning anchored to the word where you actually hear it.
- **How Words Join.** Ten plain-English construction types: kind + thing, twins glued, do + what, do + result, do + direction, person-maker, place-maker, thing-maker, sound loan, stands alone.

## Add your own words

All data lives in the `MOL` arrays near the top of the `<script>` block, one line per word:

```js
['火锅','huǒguō','hotpot','h','火:huǒ:fire,锅:guō:pot','Food'],
```

Fields: hanzi, pinyin, English, join type (`h` kind+thing, `p` twins, `v` do+what, `r` do+result, `d` do+direction, `m` person-maker, `g` place-maker, `s` thing-maker, `o` stands alone, `l` sound loan), parts as `char:pinyin:meaning` pairs, theme. Part counts and sound cards recompute automatically.

## Credits

Corpus and construction system by Sree, with lǎoshī Nianzhen (Wu Nianzhen 无念真). Built with Claude.
