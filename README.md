This site provides hosting for [Apache Fineract](https://fineract.apache.org).  An instance of https://github.com/apache/fineract/ is running on [https://demo.fineract.dev](https://demo.fineract.dev), and you can invoke e.g. [https://demo.fineract.dev/fineract-provider/actuator/health](https://demo.fineract.dev/fineract-provider/actuator/health) and the full [Apache Fineract API](https://htmlpreview.github.io/?https://github.com/apache/fineract/blob/develop/api-docs/apiLive.htm).

### Frequently Asked Questions (FAQ)

*Is this free?* The demo instance is and always will be free.

*Can I create myself a new tenant on the demo instance?*  Sure! Just to avoid any misunderstanding about what a **demo** instance is, and is not: The database of the demo instance will be completely wiped once a week by an automated script!

*Can I get a persistent non-demo tenant or full instance here?*  We're still thinking this through.  Should you have an interest in a non-demo instance of Apache Fineract, and be willing to pay for its cost, feel free to reach out to [hosting@fineract.dev](mailto:hosting@fineract.dev?subject=[www.fineract.dev]) - we're interested in understanding the need and expectations in this space.

*What version of code does this run?* The demo instance currently runs Fineract built on April 18th, 2020.  We're looking into making it auto updated from the latest `develop` branch.  [FINERACT-883](https://issues.apache.org/jira/browse/FINERACT-883) will soon let you see the exact Git revision that is running.

*What hardware, OS, DB etc. is this server running on?* It's actually not really a "server", but runs on some fancy latest generation modern cloud infrastructure.  The details shouldn't matter to users, and they may change over time, so we don't explain them in details here.

*Is this open source?*  The Fineract code that runs here of course is.  Any improvements made to be able to run this site have been and will continue to be made "[upstream first](https://www.youtube.com/watch?v=PQloi5Z-0rQ)".  The hosting setup itself is mostly manual, and there is nothing much there to share that would make much sense.  The web [page itself you are reading is on GitHub](https://github.com/vorburger/www.fineract.dev/blob/master/README.md), and you are welcome to propose any improvements to it through a pull request.

*Can you help me set up a server like this for our own use?* Depends what exactly you mean by that.  We haven't been able to figure out how to exaplain the details of how this runs and make it an effective use of your and our time.  But please do see one of the earlier questions about using this server for non-demo purposes!

*Is this Mifos?* Two things here:  1. Mifos X is the old name of the code now lives on as https://github.com/apache/fineract/ at the ASF. In that sense, yes, this server runs (the current version of the code origially known as) Mifos.  2. The Mifos Initiative ([mifos.org](https://mifos.org) is an organization supporting Apache Fineract.

*Is this an Apache Software Foundation project?* Apache Fineract sure is! This hosting website is not.


### Contact & Support

You'll most likely want to use a partner to assist you with implementing Apache Fineract software for your organization.

For community support by volunteers about how to use Apache Fineract, use:

* [mifos-users list on sourceforge.net](https://sourceforge.net/projects/mifos/lists/mifos-users) (also [on groups.google.com](https://groups.google.com/forum/#!forum/mifosusers)) for general end-user type questions
* [mifos-developer list on sourceforge.net](https://sourceforge.net/projects/mifos/lists/mifos-developer) (also on [groups.google.com](https://groups.google.com/forum/#!forum/mifosdeveloper)) for technical questions about the UI front-ends, mobile apps, etc. maintained on [github.com/openMF](https://github.com/openMF/)
* [Fineract Dev list at Apache.org](https://fineract.apache.org/) for the REST API back-end running on this server
* [issues of this project](https://github.com/vorburger/www.fineract.dev/issues) for anything specific (and only) this fineract.dev server
* [Discourse Forums offered by the Mifos Initiative](https://discourse.mifos.org)

To add new features and fix bugs blocking you in Fineract, you are cordially invited to be an active member to the open source project and contribute to the project by raising pull requests yourself. Alternatively you can pay someone to do so for you; you can meet some of the parties interested in working with you on the mailing lists.
