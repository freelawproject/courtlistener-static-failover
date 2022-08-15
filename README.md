# courtlistener-static-failover

An S3 site to be loaded when CourtListener goes down


# Upload it with

s3cmd sync ./src/ s3://cl-error-docs-static-website/errors_5xx/ --delete-removed --guess-mime-type --no-mime-magic


# A weird thing

I couldn't figure out how to make the paths work quite right, so make sure everything points to /errors_5xx/whatever.png.

You can see what I mean in the 5xx.html file.