# USPS-Webtools
Simple API for the USPS Webtools. No Authentication Required.

## Module Usage

###### Package Tracking Sample:

```python
from usps_webtools import PackageTracking

package = PackageTracking('YOUR_TRACKING_NUMBER')

package.status
package.status_last_updated
package.expected_delivery_date
package.expected_delivery_status
package.history
package.product_info
package.as_dict()

```

###### ZipTools Lookup Sample:

```python
from usps_webtools import zipByCityState, zipByAddress, cityByZip

zipByAddress('376 Fairfield St', 'New Lenox', 'IL', '60451')

zipByCityState('New Lenox', 'IL')

cityByZip('60451')


```
