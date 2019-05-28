# request_error
Contao shows request.Error and the site I was trying to reach is not avaidable

I get a Contao page with a hint that an error has occurred. The problem only occurs if I access the website in a browser for the first time and then only with "address.de", but if I access the page directly with "http://address.de", the page will show up without an error. After I have opened the page in a browser once with "http://..." from then the page works without an error with the address "address.de" as well.

In the BE under page structure the following is set:
Domain name: address.de
use https

Below you'll find the log-file record

[2019-05-20 11:11:01] request.ERROR: Uncaught PHP Exception Symfony\Component\HttpKernel\Exception\AccessDenie dHttpException: "" at /mnt/web303/a0/04/549604/htdocs/cms/vendor/symfony/http-kernel/EventListener/FragmentListener.php line 90 {"exception":"[object] (Symfony\\Component\\HttpKernel\\Exception\\Access DeniedHttpException(code: 0): at /mnt/web303/a0/04/549604/htdocs/cms/vendor/symfony/http-kernel/EventListener/FragmentListener.php:90)"} []
[2019-05-20 11:11:01] request.CRITICAL: Uncaught PHP Exception LogicException: "MemoryTokenStorage must not be accessed before it was initialized." at /mnt/web303/a0/04/549604/htdocs/cms/vendor/contao/core-bundle/src/Csrf/MemoryTokenStorage.php line 109 {"exception":"[object] (LogicException(code: 0): MemoryTokenStorage must not be accessed before it was initialized. at /mnt/web303/a0/04/549604/htdocs/cms/vendor/contao/core-bundle/src/Csrf/MemoryTokenStorage.php:109)"} []
