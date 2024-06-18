# bwdnci-oai
Public interface and descriptions for Bowdoin Collecting Institutions for Open Archives Initiative Protocol for Metadata Harvesting (OAI-PMH)

## System Details
bwdnci-oai consists of two repositories: one for our [Museum of Art Collections](https://artmuseum.bowdoin.edu) and one for our [Museum of Arctic Studies Collection](https://arcticcollections.bowdoin.edu). The repositories are built upon a Java Tomcat application that makes calls to each museums' (separate) EmbARK Collection Management System Web XML Sharing utility that exposes publicly available collection data (API). The Tomcat application converts the exposed API and transforms it to be responsive to OAI-PMH standards and protocols.

### Why separate repositories?
While we use the same Tomcat application to dispatch OAI-PMH requests and both the Art Museum (BCMA) and the Arctic Museum fall under the umbrella of _Bowdoin Collecting Institutions_, we have avoided presenting them as two sets under a single repository because their data is actually quite separate both architectually and administratively. An argument could be made for a single repository with multiple sets, but this seemed like the best way to start.

- BCMA Base URL:  (https://apps.bowdoin.edu/jbecker/oai/bcma/View.jsp)
- Arctic Base URL:  (https://apps.bowdoin.edu/jbecker/oai/arctic/View.jsp)

### Verifications
Our repository URLs pass all the validations in the OAI-PMH Validator & data-extraction tool (https://validator.oaipmh.com/)

Additionally, we have successfully tested the URLs against a harvester client phpoaipmh (https://github.com/caseyamcl/phpoaipmh)

So far, we have been unsuccessful at getting these URLs to integrate with our Alma library management system. 

![screen1](https://github.com/benicetootters/bwdnci-oai/assets/32641676/8e8c779d-d2b8-4f55-b366-6a3fed3130ae)

![screen2](https://github.com/benicetootters/bwdnci-oai/assets/32641676/5380ea78-7424-49cb-b2ba-505d0beef027)

![screen3](https://github.com/benicetootters/bwdnci-oai/assets/32641676/76e4dce3-6ebd-4d90-a858-b408b1d2e61f)

