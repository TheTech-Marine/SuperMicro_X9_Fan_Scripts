# SuperMicro_X9_Fan_Scripts
Modified for Supermicro X9 boards using an Nuvoton WPCM450 BMC

- `spincheck.sh` reads and logs temperature and fan data at a chosen interval, but does not control fans in any way. Works for both 1- and 2-zone motherboards.
- `spintest.sh` is a one-time utility that runs your fans through a range of duty cycles and logs resulting RPMs. Works for both 1- and 2-zone motherboards. The results can be used for some settings in spinpid2.sh.
- `spinpid2.sh` controls fans for motherboards with dual fan zones, peripheral and CPU/system. The zones can be reversed. Logs lots of temperature and fan data with additional CPU log.

Modified based on code from the following resources:

https://www.truenas.com/community/resources/fan-scripts-for-supermicro-boards-using-pid-logic.24/

https://www.truenas.com/community/threads/fan-scripts-for-supermicro-boards-using-pid-logic.51054/page-13#post-551335

https://gist.github.com/xontik/58d3165c670546417ab8f13d21a882fc
