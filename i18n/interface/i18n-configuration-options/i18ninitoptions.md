| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | any |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; plugins**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Collection of i18next plugins to use.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | any[] &#124; undefined |

&nbsp;&nbsp; **&#10148; skipTranslationOnMissingKey**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | boolean &#124; undefined |

&nbsp;&nbsp; **&#10148; rtEpsilon**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Leeway for computing the time difference for relative time formatting.
If abs(t1 - now) < 1 time_unit, where t1 is the date being formatted, and time_unit is a unit of time such as minute, hour etc.,
then the relative time formatting may sometime produce unexpected results, such as 'in 60 seconds' instead of 'in 1 minute'.
A non-zero rtEpsilon ensures nicer results instead. Default is 0.01. A smaller value for epsilon ensures stricter comparison.

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | number &#124; undefined |