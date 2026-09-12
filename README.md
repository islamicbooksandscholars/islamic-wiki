هدف هذا الموقع هو جمع ملخصات ودروس كتب علماء المسلمين الأكابر في مكان واحد.

هذا الموقع لايطرح حقائق تعبر عن رأي الكاتب وإنما حقائق مستقاة مباشرة من الكتب والمراجع.

كل موضوع مطروح في هذا الموقع يتضمن المصادر التي تم استخدامها في كتابة الملخص او الموضوع.

دمتم سالمين.



```dataviewjs
const groups = dv.pages('""').groupBy(p => p.file.folder);
let md = "| Directory | Files |\n| --- | --- |\n";

for (let group of groups) {
    let links = group.rows.map(r => r.file.link).join(", ");
    md += `| ${group.key || "Root"} | ${links} |\n`;
}

dv.paragraph(md);
```


