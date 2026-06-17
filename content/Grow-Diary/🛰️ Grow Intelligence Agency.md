# 🛰️ Grow Intelligence Agency (GIA)

> SCROG Operations & Cultivation Intelligence

---

# 📂 Inhaltsverzeichnis & Navigation

## ⚙️ Grow Setup

|Bereich|Link|
|---|---|
|Setup & Hilfsmittel|[[Setup und Hilfsmittel]]|
|Umweltwerte|[[Umweltwerte]]|
|Düngemittel & Werte|[[Düngemittel und Werte]]|

---

# 🌱 Aktuelle Growphase

- [x] Blüte
- [ ] Vegetation
- [ ] Seedling
---

## 🌱 Seedling

|Sorte|
|---|
|[[2 Grizzly Glue Seedling]]|
|Expert Haze|
|Blackberry Moonrocks|

---

## 🌿 Vegetation

|Sorte|
|---|
|[[2 Blackberry Moonrocks Vegi]]|
|[[2 Expert Haze Vegi]]|
|[[3 Grizzly Glue Vegi]]|

---

## 🌸 Blüte

```dataviewjs
const flip = new Date("2026-05-10");
const today = new Date();

const bt = Math.floor((today - flip) / (1000 * 60 * 60 * 24));

dv.table(
["Sorte", "Aktuell"],
[
["[[3 Blackberry Moonrocks Bloom]]", "BT" + bt],
["[[3 Expert Haze Bloom]]", "BT" + bt],
["[[4 Grizzly Glue Bloom]]", "BT" + bt]
]
);
```

---

## 🌐 Gesamtansichten

|Bereich|Link|
|---|---|
|Gesamter SCROG|[[Ganzer SCROG]]|
|TO-DO|[[TO-DO]]|

---

# ✅ Zuletzt erledigt

```tasks
done
sort by done reverse
limit 15
```