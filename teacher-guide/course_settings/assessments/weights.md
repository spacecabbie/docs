# Weights

The weights, accessed through a percentage-symbol icon ![](../../.gitbook/assets/image4.svg) on the right side of the main assessments page, allow you to define the relative importance of each of the activities within the assessment. If you don't have any activity registered at this point, return to this section when you do.

![](../../.gitbook/assets/images133%20%281%29.png)

_Illustration 108: Assessments - Weights_

We suggest that you define a distribution of weights that make a total of 100 \(or the equivalent total value for the course defined in the previous section\), otherwise it becomes really complicated to understand all the possible relative scoring issues. Several messages will remind you to do just that.

## Skills ranking <a id="skills-ranking"></a>

Skills ranking allow you to define ranks for the scores, so that they can be more easily represented literally and graphically. This option, however, **must** be enabled by your portal administrator. Otherwise you won’t see the following options.

Click on the podium icon on the right side of the main assessments page ![](../../.gitbook/assets/graphics191.png):

![](../../.gitbook/assets/graphics195.png)

_Illustration 109: Assessments – Skills ranking_

As well as a pass-mark, you can add additional options: e.g. the names you want to give to any score range to make it faster to read generic reports.

## Certificate template <a id="certificate-template"></a>

Once you have configured the rest of the tools, you might get interested in setting up your own certificate template. But before we start, let’s get 3 concepts clear:

* Certificate templates are built in HTML, so you will probably need a web designer \(or a lot of patience\) to generate beautiful templates.
* Certificate templates are build in HTML \(yes, again\), so their export to PDF \(a feature provided as a commodity in Chamilo\) might not be ideal and you might need to work over that with your designer to make sure both results are fine.
* Certificates are only generated when the certificates option is selected \(see Assessments pre-configurationon page 99\), if students have a passing grade, and if the student actually **enters** the assessment tool \(or, in 1.11, if you used the special certificate page in the learning path\)

Theassessmentstool makes it possible to create a certificate generated automatically using the learner's data stored on the platform. To set this up, click the large certificate icon ![](../../.gitbook/assets/graphics193.png) on the right side of the main page. This will bring up a screen displaying a list of existing certificates, with tool-bar options to import ![](../../.gitbook/assets/graphics194.png) or create certificates. Chamilo provides one basic template certificate that you can update if you like. Click the _Create certificate_ icon ![](../../.gitbook/assets/graphics196.png) to go to a document creation page, which allows you to design a certificate.

The page starts with a list of tags that you can use in the edition of your certificate:

![](../../.gitbook/assets/image6%20%282%29.png)_Illustration 110: Certificates edition tags_

These tags are relatively self-explanatory, but for the sake of precision, let’s define them here:

* **\(\(user\_firstname\)\)** will be replaced by the firstname of the user obtaining the certificate
* **\(\(user\_lastname\)\)** same thing as above, with the lastname
* **\(\(gradebook\_institution\)\)** this will be replaced by the name of your organization, defined by the administrator in the platform settings, and visible in the title bar of your browser
* **\(\(gradebook\_sitename\)\)** will be replaced by the name of the platform, also defined by the administrator an visible in the title bar of your browser
* **\(\(teacher\_firstname\)\)** will be replaced by the firstname of the teacher assigned to this course. A word of warning: this hasn’t been tested with multiple teachers or with sessions, so use with caution.
* **\(\(teacher\_lastname\)\)** same as above, but lastname
* **\(\(official\_code\)\)** if you use the users’ official code field, then the corresponding value will replace this tag when generating the certificate
* **\(\(date\_certificate\)\)** will be replaced by the certificate date and time, in the date format that matches your language definition
* **\(\(date\_certificate\_no\_time\)\)** same as above, without the hours and minutes
* **\(\(course\_code\)\)** if you use a clear hierarchy of course codes, using the course code here might be useful
* **\(\(course\_title\)\)** will be replaced by the course title
* **\(\(gradebook\_grade\)\)** will be replaced by the score obtained \(both absolute and percentage\) by the student
* **\(\(certificate\_link\)\)** will be replaced by the unique URL of the certificate. Chamilo keeps them well stored, so showing the link on a certificate that is going to be printed is a good idea to maintain the relationship with the digital original version
* **\(\(certificate\_link\_html\)\)** in case you will export the certificate as an HTML certificate or a PDF certificate to use in a digital format, this will put an HTML link directly on the certificate
* **\(\(certificate\_barcode\)\)** will replace the tag with a QR code with information about the certificate \(including the link to the original\). This is a very nice feature if you like QR codes, but you have to think that the tag \(a simple text on one line\) will actually be replaced by a good-size QR code. So plan the free space around this text well.
* **\(\(external\_style\)\)** and **\(\(région\)\)** are examples of extra profile fields defined on users. Extra fields will appear in this list depending on their availability, so that’s a great extension you can give to your certificates if your administrator is open to this type of usage.

Editing the certificate is then only a question of finding a good text and the right tags:

![](../../.gitbook/assets/image7%20%282%29.png)_Illustration 111: Certificate creation area_

Once you have created and saved your certificate, the main Certificate page lists the certificates that have been uploaded or created.

![](../../.gitbook/assets/image8%20%282%29.png)_Illustration 112: Certificate templates list_

You might note that the 5th icon on the right has a slightly different color for the first and the second line… That’s because the “Default certificate” in this example is still considered the… default certificate. To change that, you will have to click on the gray icon on the second line \(![](../../.gitbook/assets/graphics198.png)\) to make your new certificate \(“Future of Learning” in this example\) the default certificate for all students.

Only one certificate can be selected in a course at any one time, so choose well.

Once this is done, the magnifier icon ![](../../.gitbook/assets/image9.svg) will allow you to see a preview of the certificate with fake values. In our example, this gives something like this:

![](../../.gitbook/assets/image10%20%281%29.png)

_Illustration 113: Example certificate_

Missing something? Clearly, some HTML design with a logo, the names of the people approving this certificate would have been a good addition. You will find these on the certificate available in every course in Chamilo by default, which would render like this.

![](../../.gitbook/assets/image11%20%282%29.png)_Illustration 114: Default certificate template available in Chamilo_

As you can see, this template is much more developed than the quick template we built as an example for this guide. That’s because we intent to provide you with the best tools and templates to ensure you can generate a great impact with your course with minimal effort. You can edit the default template if you want and replace the logo by your institution’s logo. This is all up to you.

This certificate, however, sometimes shows a little defect when exporting to PDF, so test it first if you expect this to be your best feature...

You can return to the assessments screen through the breadcrumb navigation \(click _Assessments_\).

