# Glossary

## item status

<span id='status'></span>

| status | before/after version | description | worker | workspace |
| :--- | :--- | :--- | :--- | :--- |
| unallocated | before | need allocate | master | allocation |
| untranslated | before | need first translate | translator | translation |
| re-transalted | before | need another translate | translator | re-translation |
| unreviewed | before | need reivewed | reviewer | review |
| qualified | before | is approved | reviewer | review |
| conflict | after | correctness is suspected. | master | conflict handle |
| error | after | marked wrong | master | conflict handle |



