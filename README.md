This site provided hosting for [Apache Fineract](https://fineract.apache.org), and runs the code from [github.com/apache/fineract](https://github.com/apache/fineract/) as a service.

<!--
### Usage

Open the [Community App UI](https://openmf.github.io/community-app?baseApiUrl=https://demo.fineract.dev&tenantIdentifier=default) (older, but more complete; see [github.com/openMF/community-app](https://github.com/openMF/community-app)) or [the Web App UI](https://openmf.github.io/web-app/) (newer, see [github.com/openMF/web-app](https://github.com/openMF/web-app/)) and login with e.g. _mifos/password_.

You can also directly invoke [Apache Fineract's REST API](https://demo.fineract.dev/fineract-provider/api-docs/apiLive.htm) backend on this server; e.g. via [/api/v1/clients](https://demo.fineract.dev/fineract-provider/api/v1/clients?tenantIdentifier=default) or the [api/v1/audits](https://demo.fineract.dev/fineract-provider/api/v1/audits?tenantIdentifier=default) etc. or by [using the new Swagger UI](https://demo.fineract.dev/fineract-provider/swagger-ui/index.html) (or directly use [Fineract's Swagger YAML](https://demo.fineract.dev/fineract-provider/swagger-ui/fineract.yaml) in a tool).  Again, always login with e.g. _mifos/password_ to the REST API, just like the UI.
-->

### Frequently Asked Questions (FAQ)

*Is this free?*  The demo instance was free.

*Who pays for hosting this?*  [vorburger@](https://github.com/vorburger) originally paid for it personally.  Google Cloud hosting costs for this demo site were graciously offered by [Google Open Source](https://opensource.google/) from mid October 2021 to 2022.  The demo instance is currently stopped; please reach out to [hosting@fineract.dev](mailto:hosting@fineract.dev?subject=[www.fineract.dev]) if you would like to discuss bringing it back alive.

*Can I do whatever I like on the demo instance?*  Sure! Just to avoid any misunderstanding about what a **demo** is, and is not: The database of the default tenant on the demo may be completely wiped about once a week by an automated script!

*Can I get a persistent non-demo tenant or full instance here?*  We're still thinking this through.  Should you have an interest in a non-demo instance of Apache Fineract, please reach out to [hosting@fineract.dev](mailto:hosting@fineract.dev?subject=[www.fineract.dev]) - we're interested in understanding the need and expectations in this space.

*What version of code does this run?*  This server uses CI/CD and always automatically updates itself from the very latest source code available on the `develop` branch of Fineract ([FINERACT-970](https://issues.apache.org/jira/browse/FINERACT-970)).  You can verify this for yourself by [checking the /actuator/info API](https://demo.fineract.dev/fineract-provider/actuator/info), which returns the exact Git commit revision that is running.  (New deployments take about 15' after we merge Pull Requests.)

*How well tested is the code that this site runs?*  All running code has passed all of Fineract's unit and integration tests of the respective code branch.  (Any unstable tests which had to be disabled during development, are therefore, of course, not run before code deploys to this server.)

*What hardware, OS, DB etc. is this server running on?*  It's actually not really a "server", but runs on latest generation modern cloud infrastructure.  The [Running Fineract.dev, SRE style](https://docs.google.com/presentation/d/1-VP4bNkc5kZ3B0yme_vYLiY1qpswnfz8ainnX5fp3l8/) presentation given at ApacheCon has some background (and [this blog post about how to manage GitHub secrets on repos you only have Write but not Admin](http://blog2.vorburger.ch/2020/05/fineractdev-cicd-from-github-to-google.html)). The exact details shouldn't matter to users, and they may change over time, so we don't explain them in details here.  The DB is MySQL 8.0 on Google Cloud SQL (since [#8](https://github.com/vorburger/www.fineract.dev/issues/8)), and using the MariaDB (not MySQL, nor Drizzle; see [FINERACT-982](https://issues.apache.org/jira/browse/FINERACT-982)) JDBC driver that Fineract includes in its Docker container.

*Can I get access to the Fineract logs from this server?* It depends. If you are an active Apache Fineract committer and want to help with [FINERACT-932](https://issues.apache.org/jira/browse/FINERACT-932) kind of work and could benefit from access to Google Cloud Error Reporting for this server, [then yes - just ask](https://github.com/vorburger/www.fineract.dev/issues/9).

*If this runs on the cloud, will it be always available?*  The cloud infrastructure  that this runs on is very reliable, and will e.g. "auto heal" and restart crashed instances.  The HTML/JS is served from a world-wide content distribution network (CDN).  We use top notch industry standard [Site Reliability Engineering](https://landing.google.com/sre/books/) (SRE) best practices such as monitoring metrics etc. to keep an eye on this server.  But here is a fun idea: Try to crash our demo - and if you manage, then work with us in the open source project to make the Fineract code more scaleable and reliable!

*Is this open source?*  The Fineract and UI code that runs here of course is.
Many improvements made to be able to run this site already have been and will continue to be made "[upstream first](https://www.youtube.com/watch?v=PQloi5Z-0rQ)".  The hosting setup itself is mostly manual, and there is nothing much there to share that would make much sense.  The web [page itself you are reading is on GitHub](https://github.com/vorburger/www.fineract.dev/blob/master/README.md), and you are welcome to propose any improvements to it through a pull request.

*Can you help me set up a server like this for our own use?*  Depends what exactly you mean by that.  We haven't been able to figure out how to explain the details of how this runs and make it an effective use of your and our time.  Having said that, please see the earlier questions about using this server for non-demo purposes.  If that is not an option for you, we would be interested in understanding why.

*Is this Mifos?*  Two things here:  1. Mifos X is the old name of the code which now lives on at [https://github.com/apache/fineract](https://github.com/apache/fineract/)  at the ASF. In that sense, yes, this server runs (the current version of the code origially known as) Mifos.  2. The [Mifos.org](https://mifos.org) Initiative is the organization which originally helped move Mifos X to the Apache Foundation, and which continues to actively support the Apache Fineract project in many ways.

*Is this an Apache Software Foundation project?* Apache Fineract sure is! This hosting website is not.

*Is this [Fineract CN](https://github.com/search?q=org%3Aapache+fineract-cn&unscoped_q=fineract-cn)?* No, this site curently runs only [Fineract](https://github.com/apache/fineract).


### Contact & Support

You'll most likely want to use a partner to assist you with implementing Apache Fineract software for your organization.

For community support by volunteers about how to use Apache Fineract, use:

* [mifos-users list on sourceforge.net](https://sourceforge.net/projects/mifos/lists/mifos-users) (also [on groups.google.com](https://groups.google.com/forum/#!forum/mifosusers)) for general end-user type questions
* [mifos-developer list on sourceforge.net](https://sourceforge.net/projects/mifos/lists/mifos-developer) (also on [groups.google.com](https://groups.google.com/forum/#!forum/mifosdeveloper)) for technical questions about the UI front-ends, mobile apps, etc. maintained on [github.com/openMF](https://github.com/openMF/)
* [Fineract Dev list at Apache.org](https://fineract.apache.org/) for the REST API back-end running on this server
* [Issues of this project](https://github.com/vorburger/www.fineract.dev/issues) for anything specific (and only) to this fineract.dev server
* [Discourse Forums offered by the Mifos Initiative](https://discourse.mifos.org)

To add new features and fix bugs blocking you in Fineract, you are cordially invited to be an active open source contributor to the Apache Fineract project.  Alternatively you can pay someone to do so for you; you can meet some of the parties interested in working with you on the mailing lists.
