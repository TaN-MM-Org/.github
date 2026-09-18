---
name: Wrong-number report
about: A quantity the package computed disagrees with a published value,
  a textbook result, or your measurement. The most valuable report we can get.
title: "[wrong number] "
labels: wrong-number
---

**What did the package compute, and what should it be?**

The value you got, the value you expected, and the source of the
expected value (paper with DOI, textbook with edition and page, or
your measurement with its error bar).

**Minimal script**

The smallest runnable snippet that produces the number, including the
package version (`python -c "import <pkg>; print(<pkg>.__version__)"`).

**Units and conventions**

If there is any chance the two numbers use different units, sign
conventions, or reference planes, say which ones each side uses. Most
wrong-number reports are convention mismatches -- those are
documentation bugs on our side, and we fix them as such.
