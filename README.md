This site provides hosting for code from [Apache Fineract](https://fineract.apache.org), and runs [github.com/apache/fineract](https://github.com/apache/fineract/) as a service.
It also provides [github.com/openMF/community-app](https://github.com/openMF/community-app) and [github.com/openMF/web-app](https://github.com/openMF/web-app/).


### Usage

Open [cui.fineract.dev](https://cui.fineract.dev/?baseApiUrl=https://demo.fineract.dev&tenantIdentifier=default) (Community App, old) or [wui.fineract.dev](https://wui.fineract.dev) (Web App, new) and login to both with _mifos/password_.

You can also invoke [Apache Fineract's REST API](https://demo.fineract.dev/fineract-provider/api-docs/apiLive.htm) backend directly; e.g. [/api/v1/clients](https://demo.fineract.dev/fineract-provider/api/v1/clients?tenantIdentifier=default) or the [api/v1/audits](https://demo.fineract.dev/fineract-provider/api/v1/audits?tenantIdentifier=default) (login with _mifos/password_ for both), etc.


### Frequently Asked Questions (FAQ)

*Is this free?*  The demo instance is and always will be free.

*Can I do whatever I like on the demo instance?*  Sure! Just to avoid any misunderstanding about what a **demo** is, and is not: The database of the default tenant on the demo may be completely wiped about once a week by an automated script!

*Can I get a persistent non-demo tenant or full instance here?*  We're still thinking this through.  Should you have an interest in a non-demo instance of Apache Fineract, please reach out to [hosting@fineract.dev](mailto:hosting@fineract.dev?subject=[www.fineract.dev]) - we're interested in understanding the need and expectations in this space.

*What version of code does this run?*  This server uses CI/CD and always automatically updates itself from the very latest source code available on the `develop` branch of Fineract ([FINERACT-970](https://issues.apache.org/jira/browse/FINERACT-970)).  You can verify this for yourself by [checking the /actuator/info API](https://demo.fineract.dev/fineract-provider/actuator/info), which returns the exact Git commit revision that is running.  (New deployments take about 15' after we merge Pull Requests.)

*How well tested is the code that this site runs?*  All running code has passed all of Fineract's unit and integration tests of the respective code branch.  (Any unstable tests which had to be disabled during development, are therefore, of course, not run before code deploys to this server.)

*What hardware, OS, DB etc. is this server running on?*  It's actually not really a "server", but runs on latest generation modern cloud infrastructure.  The full details shouldn't matter to users, and they may change over time, so we don't explain them in details here.

*If this runs on the cloud, will it be always available?*  The cloud infrastructure  that this runs on is very reliable, and will e.g. "auto heal" and restart crashed instances.  The HTML/JS is served from a world-wide content distribution network (CDN).  We use top notch industry standard [Site Reliability Engineering](https://landing.google.com/sre/books/) (SRE) best practices such as monitoring metrics etc. to keep an eye on this server.  But here is a fun idea: Try to crash our demo - and if you manage, then work with us in the open source project to make the Fineract code more scaleable and reliable!

*Is this open source?*  The Fineract and UI code that runs here of course is
([patched](https://github.com/openMF/community-app/compare/develop...vorburger:firebase), and
[patched](https://github.com/openMF/web-app/compare/master...vorburger:fineract.dev)).
Many improvements made to be able to run this site already have been and will continue to be made "[upstream first](https://www.youtube.com/watch?v=PQloi5Z-0rQ)".  The hosting setup itself is mostly manual, and there is nothing much there to share that would make much sense.  The web [page itself you are reading is on GitHub](https://github.com/vorburger/www.fineract.dev/blob/master/README.md), and you are welcome to propose any improvements to it through a pull request.

*Can you help me set up a server like this for our own use?*  Depends what exactly you mean by that.  We haven't been able to figure out how to explain the details of how this runs and make it an effective use of your and our time.  Having said that, please see the earlier questions about using this server for non-demo purposes.  If that is not an option for you, we would be interested in understanding why.

*Is this Mifos?*  Two things here:  1. Mifos X is the old name of the code which now lives on at [https://github.com/apache/fineract](https://github.com/apache/fineract/)  at the ASF. In that sense, yes, this server runs (the current version of the code origially known as) Mifos.  2. The [Mifos.org](https://mifos.org) Initiative is the organization which originally helped move Mifos X to the Apache Foundation, and which continues to actively support the Apache Fineract project in many ways.

*Is this an Apache Software Foundation project?* Apache Fineract sure is! This hosting website is not.


### Contact & Support

You'll most likely want to use a partner to assist you with implementing Apache Fineract software for your organization.

For community support by volunteers about how to use Apache Fineract, use:

* [mifos-users list on sourceforge.net](https://sourceforge.net/projects/mifos/lists/mifos-users) (also [on groups.google.com](https://groups.google.com/forum/#!forum/mifosusers)) for general end-user type questions
* [mifos-developer list on sourceforge.net](https://sourceforge.net/projects/mifos/lists/mifos-developer) (also on [groups.google.com](https://groups.google.com/forum/#!forum/mifosdeveloper)) for technical questions about the UI front-ends, mobile apps, etc. maintained on [github.com/openMF](https://github.com/openMF/)
* [Fineract Dev list at Apache.org](https://fineract.apache.org/) for the REST API back-end running on this server
* [issues of this project](https://github.com/vorburger/www.fineract.dev/issues) for anything specific (and only) this fineract.dev server
* [Discourse Forums offered by the Mifos Initiative](https://discourse.mifos.org)

To add new features and fix bugs blocking you in Fineract, you are cordially invited to be an active open source contributor to the Apache Fineract project.  Alternatively you can pay someone to do so for you; you can meet some of the parties interested in working with you on the mailing lists.
