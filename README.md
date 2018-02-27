# 386test
386(a nickname) is a funny guy as the "symbol" of "Loongson Club" QQ group. He hold a  hilarious opinion that Loongson 3 processors is worth than Intel P4 series processors.(This point is sightly wrong for us,  Loongson 3 is a modern advanced high-performance processor while P4 is outdated for a long time).

He proposed these tests to examine the performance of Loongson3. Although they're not very fair at all. But they help us find out some choke poins .

All these tests are arch and os indepedent so we can test on any systems. PRs and issues for test results are welcomed.

For GCC we recommand to add  "-O3 -static" in CFLAG.

For all these tests, we compare time costed in final output to compare the performance.

## Test1 integal
This test mainly tests the float point performance of processor.
Libm is used for sin claculation except MIPS.
Trough this test we found the float point performance of Glibc on MIPS is unbelievable slow and need to be optimized.

##Test2 Pi
This test claculates Pi to test the INT performance of processor.
We test 9999 digits of Pi.