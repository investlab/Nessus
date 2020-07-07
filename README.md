# Change download Nessus file
- From: https://www.tenable.com/downloads/api/v1/public/pages/nessus/downloads/10444/download?i_agree_to_tenable_license_agreement=true
- To: Newest version in https://www.tenable.com/downloads/nessus?loginAttempted=true

# Build image:
- docker build --squash -t nessus:v1 -f Dockerfile .

# Run image to container:
- docker run -it --name nessus1 -p 8834:8834 -d nessus:v1
