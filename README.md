# LeGO-LOAM (ros2 에서 빌드중 ,,,)

error: ‘library_version_type’ in namespace ‘boost::serialization’ does not name a type

위의 오류는 아래의 코드를 ``` sudo nano /usr/include/boost/serialization/list.hpp ```에 삽입

```
#if BOOST_VERSION >= 107400
#include <boost/serialization/library_version_type.hpp>
#endif
```
