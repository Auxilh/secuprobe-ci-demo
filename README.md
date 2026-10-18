# SecuProbe CI demo — github

Demonstrates SecuProbe in GitHub Actions (`Auxilh/secuprobe-scan-action@v1.1.0`).

Every pull request and every push to `main` scans `https://demo-vuln.secuprobe.io`, an
**intentionally vulnerable** demo target that exposes fake sensitive files. The pipeline is expected
to **fail**: the scan reports critical findings and the threshold is `critical`. On a pull request,
SecuProbe posts one comment with the new and fixed findings and a link to the report.

Documentation: https://secuprobe.io/docs/api
