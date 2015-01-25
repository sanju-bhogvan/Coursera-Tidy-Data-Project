
    
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a id="user-content-getting-and-cleaning-data" class="anchor" href="#getting-and-cleaning-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Getting and Cleaning Data</h1>

<h2>
<a id="user-content-course-project" class="anchor" href="#course-project" aria-hidden="true"><span class="octicon octicon-link"></span></a>Course Project</h2>

<p>You should create one R script called run_analysis.R that does the following.</p>

<ol class="task-list">
<li>Merges the training and the test sets to create one data set.</li>
<li>Extracts only the measurements on the mean and standard deviation for each measurement.</li>
<li>Uses descriptive activity names to name the activities in the data set</li>
<li>Appropriately labels the data set with descriptive activity names.</li>
<li>Creates a second, independent tidy data set with the average of each variable for each activity and each subject.</li>
</ol>

<h2>
<a id="user-content-steps-to-work-on-this-course-project" class="anchor" href="#steps-to-work-on-this-course-project" aria-hidden="true"><span class="octicon octicon-link"></span></a>Steps to work on this course project</h2>

<ol class="task-list">
<li>Download the data source and put into a folder on your local drive. You'll have a <code>UCI HAR Dataset</code> folder.</li>
<li>Put <code>run_analysis.R</code> in the parent folder of <code>UCI HAR Dataset</code>, then set it as your working directory using <code>setwd()</code> function in RStudio.</li>
<li>Run <code>source("run_analysis.R")</code>, then it will generate a new file <code>tiny_data.txt</code> in your working directory.</li>
</ol>

<h2>
<a id="user-content-dependencies" class="anchor" href="#dependencies" aria-hidden="true"><span class="octicon octicon-link"></span></a>Dependencies</h2>

<p><code>run_analysis.R</code> file will help you to install the dependencies automatically. It depends on <code>reshape2</code> and <code>data.table</code>. </p>
</article>
  </div>

  </div>
</div>

