


```dataviewjs
const flip = new Date("2026-05-10");
const today = new Date();

const bt = Math.floor((today - flip) / (1000 * 60 * 60 * 24));

const progress = (
(bt/60)*100 +
(bt/67)*100 +
(bt/60)*100
) / 3;

const p = Math.min(100, progress);

const filled = Math.round(p / 10);
const bar = "█".repeat(filled) + "░".repeat(10-filled);

dv.paragraph(`## 🌱 Gesamtfortschritt`);
dv.paragraph(`**${p.toFixed(1)}%**`);
dv.paragraph(bar);
```


```dataviewjs
const flip = new Date("2026-05-10");
const today = new Date();

const bt = Math.floor((today - flip) / (1000 * 60 * 60 * 24));

const strains = [
["[[3 Blackberry Moonrocks Bloom]]", 60],
["[[3 Expert Haze Bloom]]", 67],
["[[4 Grizzly Glue Bloom]]", 60]
];

function indicator(days){
    if(days > 21) return "🟢";
    if(days > 7) return "🟡";
    return "🔴";
}

dv.table(
["Sorte", "Aktuell", "Countdown"],
strains.map(s => {
    const remaining = s[1] - bt;
    return [
        s[0],
        `BT${bt}`,
        `${indicator(remaining)} ${remaining} Tage`
    ];
})
);
```


