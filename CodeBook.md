  
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a id="user-content-codebook" class="anchor" href="#codebook" aria-hidden="true"><span class="octicon octicon-link"></span></a>CodeBook</h1>

<p>This is a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data.</p>

<h2>
<a id="user-content-the-data-source" class="anchor" href="#the-data-source" aria-hidden="true"><span class="octicon octicon-link"></span></a>The data source</h2>

<ul class="task-list">
<li>Original data: <a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a>
</li>
<li>Original description of the dataset: <a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones</a>
</li>
</ul>

<h2>
<a id="user-content-data-set-information" class="anchor" href="#data-set-information" aria-hidden="true"><span class="octicon octicon-link"></span></a>Data Set Information</h2>

<p>The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.</p>

<p>The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.</p>

<h2>
<a id="user-content-the-data" class="anchor" href="#the-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>The data</h2>

<p>The dataset includes the following files:</p>

<ul class="task-list">
<li><p>'README.txt'</p></li>
<li><p>'features_info.txt': Shows information about the variables used on the feature vector.</p></li>
<li><p>'features.txt': List of all features.</p></li>
<li><p>'activity_labels.txt': Links the class labels with their activity name.</p></li>
<li><p>'train/X_train.txt': Training set.</p></li>
<li><p>'train/y_train.txt': Training labels.</p></li>
<li><p>'test/X_test.txt': Test set.</p></li>
<li><p>'test/y_test.txt': Test labels.</p></li>
</ul>

<p>The following files are available for the train and test data. Their descriptions are equivalent.</p>

<ul class="task-list">
<li><p>'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.</p></li>
<li><p>'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.</p></li>
<li><p>'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.</p></li>
<li><p>'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.</p></li>
</ul>

<h2>
<a id="user-content-transformation-details" class="anchor" href="#transformation-details" aria-hidden="true"><span class="octicon octicon-link"></span></a>Transformation details</h2>

<p>There are 5 parts:</p>

<ol class="task-list">
<li>Merges the training and the test sets to create one data set.</li>
<li>Extracts only the measurements on the mean and standard deviation for each measurement.</li>
<li>Uses descriptive activity names to name the activities in the data set</li>
<li>Appropriately labels the data set with descriptive activity names.</li>
<li>Creates a second, independent tidy data set with the average of each variable for each activity and each subject.</li>
</ol>

<h2>
<a id="user-content-how-run_analysisr-implements-the-above-steps" class="anchor" href="#how-run_analysisr-implements-the-above-steps" aria-hidden="true"><span class="octicon octicon-link"></span></a>How <code>run_analysis.R</code> implements the above steps:</h2>

<ul class="task-list">
<li>Require <code>reshape2</code> and <code>data.table</code> librareis.</li>
<li>Load both test and train data</li>
<li>Load the features and activity labels.</li>
<li>Extract the mean and standard deviation column names and data.</li>
<li>Process the data. There are two parts processing test and train data respectively.</li>
<li>Merge data set.</li>
</ul>
</article>
  </div>

  </div>
</div>
