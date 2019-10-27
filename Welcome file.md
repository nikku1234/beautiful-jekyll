---


---

<h1 id="configuration-for-mac---xcode">Configuration for Mac - Xcode</h1>
<p>This article is about how to configure Xcode env for running OpenCv with C++ projects.</p>
<h1 id="terminal">Terminal</h1>
<ol>
<li>
<p>Install Xcode v10.2</p>
</li>
<li>
<p>Install Command Line Tools</p>
<pre><code> xcode-select --install
</code></pre>
</li>
<li>
<p>Install homebrew</p>
<pre><code> /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
</code></pre>
</li>
<li>
<p>Install OpenCV</p>
<pre><code> brew install opencv
</code></pre>
</li>
</ol>
<p>OpenCV located at “/usr/local/Cellar/opencv/”</p>
<ul>
<li>
<p>To remove</p>
<pre><code>brew rm opencv
</code></pre>
</li>
<li>
<p>To update all installed packages</p>
<pre><code>brew update &amp;&amp; brew upgrade &amp;&amp; brew cleanup
</code></pre>
</li>
</ul>
<ol start="5">
<li>
<p>Install pkg-config</p>
<pre><code> brew install pkg-config
</code></pre>
<p>pkg-config located at /usr/local/lib/pkgconfig/ where containing symlink to package, checking opencv4.pc exist or not.</p>
</li>
</ol>
<p>If opencv4.pc does not exist, make a symlink:</p>
<ul>
<li>
<p>Put to ./bash_profile</p>
<pre><code>export PKG_CONFIG_PATH=/usr/local/lib/pkgconfig/
</code></pre>
</li>
<li>
<p>Make a symlink</p>
<pre><code>ln -s /usr/local/Cellar/opencv/4.0.1/lib/pkgconfig/opencv4.pc $PKG_CONFIG_PATH
</code></pre>
</li>
</ul>
<ol start="6">
<li>
<p>Check OpenCV linker flags</p>
<pre><code> pkg-config --cflags --libs opencv4
</code></pre>
</li>
</ol>
<p>Look like this:</p>
<p>-I/usr/local/Cellar/opencv/4.0.1/include/opencv4/opencv -I/usr/local/Cellar/opencv/4.0.1/include/opencv4 -L/usr/local/Cellar/opencv/4.0.1/lib -lopencv_gapi -lopencv_stitching -lopencv_aruco -lopencv_bgsegm -lopencv_bioinspired -lopencv_ccalib -lopencv_dnn_objdetect -lopencv_dpm -lopencv_face -lopencv_fuzzy -lopencv_hfs -lopencv_img_hash -lopencv_line_descriptor -lopencv_reg -lopencv_rgbd -lopencv_saliency -lopencv_stereo -lopencv_structured_light -lopencv_phase_unwrapping -lopencv_superres -lopencv_optflow -lopencv_surface_matching -lopencv_tracking -lopencv_datasets -lopencv_dnn -lopencv_plot -lopencv_videostab -lopencv_video -lopencv_xfeatures2d -lopencv_shape -lopencv_ml -lopencv_ximgproc -lopencv_xobjdetect -lopencv_objdetect -lopencv_calib3d -lopencv_features2d -lopencv_highgui -lopencv_videoio -lopencv_imgcodecs -lopencv_flann -lopencv_xphoto -lopencv_photo -lopencv_imgproc -lopencv_core</p>
<ul>
<li>
<p>If you get an error, then change opencv4 to opencv</p>
<pre><code>pkg-config --cflags --libs opencv
</code></pre>
</li>
<li>
<p>If still error, you might need to specify the location of opencv.pc file</p>
<pre><code>  pkg-config --cflags --libs path/to/opencv.pc
</code></pre>
</li>
</ul>
<p>Ex:</p>
<pre><code>pkg-config --cflags --libs /usr/local/Cellar/opencv/4.0.1/lib/pkgconfig/opencv4.pc
</code></pre>
<h2 id="xcode-config">Xcode Config</h2>
<ul>
<li>Open Xcode -&gt; New Project -&gt; macOS -&gt; Command Line Tool -&gt; Next -&gt; Select language C++</li>
<li>Edit project running scheme -&gt; Run -&gt; Options -&gt; Check on Working Directory to Use custom working directory with the path of current source files folder. -&gt; Close</li>
<li>Edit Scheme</li>
<li>
<ul>
<li>
<p>Select Project -&gt; Build Settings -&gt;Header Search Paths: 			/usr/local/Cellar/opencv/4.1.2/include (recursive)</p>
</li>
<li>
<p>Library Search Paths: /usr/local/Cellar/opencv/4.1.2/lib (recursive)</p>
</li>
<li>
<p>Other Linker Flags: Insert all content from ‘pkg-config — cflags — libs opencv4’</p>
<p>Content like:</p>
<pre><code>  -I/usr/local/Cellar/opencv/4.0.1/include/opencv4/opencv -I/usr/local/Cellar/opencv/4.0.1/include/opencv4 -L/usr/local/Cellar/opencv/4.0.1/lib -lopencv_gapi -lopencv_stitching -lopencv_aruco -lopencv_bgsegm -lopencv_bioinspired -lopencv_ccalib -lopencv_dnn_objdetect -lopencv_dpm -lopencv_face -lopencv_fuzzy -lopencv_hfs -lopencv_img_hash -lopencv_line_descriptor -lopencv_reg -lopencv_rgbd -lopencv_saliency -lopencv_stereo -lopencv_structured_light -lopencv_phase_unwrapping -lopencv_superres -lopencv_optflow -lopencv_surface_matching -lopencv_tracking -lopencv_datasets -lopencv_dnn -lopencv_plot -lopencv_videostab -lopencv_video -lopencv_xfeatures2d -lopencv_shape -lopencv_ml -lopencv_ximgproc -lopencv_xobjdetect -lopencv_objdetect -lopencv_calib3d -lopencv_features2d -lopencv_highgui -lopencv_videoio -lopencv_imgcodecs -lopencv_flann -lopencv_xphoto -lopencv_photo -lopencv_imgproc -lopencv_core
</code></pre>
</li>
</ul>
</li>
</ul>

