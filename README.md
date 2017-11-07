TASK DATE: 07.11.2017 - FINISHED: 07.11.2017

TASK SHORT DESCRIPTION: 1181 (Move "Short enticing description" to beneath the title of a news story, above the image.)

GITHUB REPOSITORY CODE: hotfix/task-1181-move-short-enticing-description

ORIGINAL WORK: https://github.com/BusinessBecause/network-site/tree/hotfix/task-1181-move-short-enticing-description

	CHANGES
 
		IN FILES: 
			
			C:\toucantech.dev\network-site\addons\default\modules\news\views\view.php

				CHANGED CODE: 
					
					FROM: 
				
						<p class="news_image_intro"><?=$post->intro?></p>
						
					TO + removed: 
					
						<?php if (trim($post->intro) != '') : ?>
							<p class="news_image_intro"><?=$post->intro?></p>
						<?endif;?>	
						
			C:\toucantech.dev\network-site\addons\default\modules\news\css\news.css
			
				ADDED CODE: 
				
					p.news_image_intro {
						margin: 0px 0px 10px 0px;
						font-size: 14px;
						text-align: justify;
					}
