# Sane Database Change Management with Sqitch

SQL change management is **hard.** Most “migration”-style implementations require opaque naming conventions, prefer DSLs that cover a fraction of SQL, and require duplication of code for simple changes to existing functions. Such does not have to be. And now it’s not

Introducing Sqitch, simple SQL change management that doesn’t suck. Sqitch doesn’t care what programming language your app is written in. It has no opinions as to what database to use or what its schema should look like. And it doesn’t require sequentially-named migration scripts or the use of any DSL other than SQL. Sqitch lets you to write SQL migration scripts that target your database, and provides a simple, unintrusive interface for specifying dependencies, so that it can run things in the proper order.

So come to this talk to learn all about Sqitch: How it works, where to get it, and how to get the most out of managing database deployments.

David Wheeler is Senior Data Architect at iovation and an associate at [PGExperts](http://www.pgexperts.com/). He is responsible, among other things, for [PGXN](http://pgxn.org/), [pgTAP](http://pgtap.org/), [DesignScene](http://www.designsceneapp.com/), and way too many [CPAN modules](https://metacpan.org/author/DWHEELER). He lives in Portland unless he’s traveling with his family.
