upload: $(HTML)
	rsync -v -c -e ssh -r --exclude '.*' --exclude '.*/' --exclude '*~' --exclude '#*#' --exclude '*.m4' --exclude private/ --exclude Makefile --exclude README.md . login.academicweb.nd.edu:www/teaching/theory/2026

oldupload:
	lftp dchiang@www3ftps.nd.edu -e 'mirror -vvv -R -L -X .* -X .*/ -I .htaccess -X *~ -X\#*\# -X *.m4 -X private/ -X Makefile -X README.md . www/teaching/theory/2026; quit'
