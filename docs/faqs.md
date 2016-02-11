# <center><span style="color:#428bca"> FAQs </span></center>
<hr style="background:#428bca; border:0; height:2px" />

<div class="tab-pane active in fade" id="faq-cat-1">
    <div class="panel-group" id="accordion-cat-1">
        <div class="panel panel-default panel-faq">
            <div class="panel-heading">
                <a data-toggle="collapse" data-parent="#accordion-cat-1" href="#faq-1">
                    <h4 class="panel-title">
                        <span style="color:ForestGreen"> Xcode Build Failed </span>
                        <span class="pull-right"><i class="fa fa-arrows-v"></i></span>
                    </h4>
                </a>
            </div>
            <div id="faq-1" class="panel-collapse collapse">
                <div class="panel-body">
					When I run it in Xcode I'm getting a "Build Failed" error, with message:
					<ul>
						<li>
							ld: library not found for -lRNVectorIcons
						</li>
						<li>
							clang: error: linker command failed with exit code 1 (use -v to see invocation)
						</li>
					</ul>
				</div>
				<div class="panel-footer">
					<b> Probabilities </b>
					<ul>
						<li> This might be the problem if you have <span style="color:#d14">'npm3'</span> installed in your system. </li>
						<li> Make sure you have installed <span style="color:#d14">'npm2'</span>. </li>
						<li> Linking the Vector Icons repo in XCode will solve the issue </li>
					</ul> <br />
					<b> Solution 1: Drag-drop to link RN Vector Icons files</b>
					<ul>
						<li> In your finder / computer, navigate to <span style="color:#d14">'NativeStarter'</span>(project folder) -> node_modules -> react-native-vector-icons </li>
						<li> Drag the <span style="color:#d14">'RNVectorIcons.xcodeproj'</span> to the Libraries in the sidebar as explained in the image below </li>
					</ul> <br />
					<br /><br /><b> Solution 2: Manually link the RN Vector Icons files</b>
					Steps:<br />
					<ul>
						<li> Go to <span style="color:#d14">'Build Phases'</span> in Xcode </li>
						<li> Link Binaries with Libraries by clicking on <span style="color:#d14">'+'</span> </li>
						<li> Click on <span style="color:#d14">'Add Other'</span> </li>
						<li> Navigate to <span style="color:#d14">'NativeStarter'</span> (project folder) -> node_modules -> react-native-vector-icons </li>
						<li> Select <span style="color:#d14">'RNVectorIcons.xcodeproj'</span> </li>
						<li> Clean Build </li>
						<li> Build Again </li>
					</ul> <br />
				</div>
            </div>
        </div>
        <div class="panel panel-default panel-faq">
            <div class="panel-heading">
                <a data-toggle="collapse" data-parent="#accordion-cat-1" href="#faq-2">
                    <h4 class="panel-title">
                        <span style="color:ForestGreen"> Watchman Error </span>
                        <span class="pull-right"><i class="fa fa-arrows-v"></i></span>
                    </h4>
                </a>
            </div>
            <div id="faq-2" class="panel-collapse collapse">
                <div class="panel-body">
					I am getting a watchman error when I run npm install.
				</div>
				<div class="panel-footer">
					<b>Solution:</b> 
					<ul>
						<li> Update <span style="color:#d14">'watchman'</span> to the latest version. </li>
						<li> Run <span style="color:#d14">'npm'</span> install again. </li>
					</ul>
				</div>
            </div>
        </div>
    </div>
</div>








