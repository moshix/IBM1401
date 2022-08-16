[![Discord](https://img.shields.io/discord/423767742546575361.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/vpEv3HJ)
<img alt="Linux" src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">


# IBM 1401 EMULATOR IN BAL 360 ASSEMBLY

This is an emulator for the venerable IBM 1401 mainframe computer of the early 60s. 

It is written in S/360 assembler and assembles with some (for me) unresolvable problems with the Waterloo University Assembler G for  MVS 3.8. You can find the Assembler G here: http://www.jaymoseley.com/hercules/compilers/list_of.htm#ASMG27A

The original code we had on this repo didn't assemble cleanly. After work from Bernard Murphy, Gerard Postpischil and others it now cleanly assembles.

Instructions on how to run the emulator are in the code itself, but I shall write up a manual, and also make a youtube video available on how to get it to run. 

<pre>

     1 4 0 1   S I M U L A T O R   F O R   S Y S T E M / 3 6 0       * 00000500

                                                                     * 00000600

                                                                     * 00000700


                                                                     * 00000800


     THIS PROGRAM WILL SIMULATE A 1401 ON A SYSTEM/360.  THE         * 00000900


 SYSTEM/360 MUST HAVE AT LEAST 65K, STANDARD INSTURCTION SET, ONE    * 00001000

 1052, ONE 2540, AND ONE PRINTER. THE 1401 FEATURES SUPPORTED ARE    * 00001100

 ADVACED PROGRAMMING, SENSE SWITCHES, TAPES, MULTIPLY, DIVIDE,       * 00001200

 16K CORE, AND ALL STANDARD INSTRUCTIONS EXCEPT SELECT STACKER.      * 00001300

 OPERATOR CONTROL IS THROUGH THE 1052, USING THE FOLLOWING ENTRIES   * 00001400

                                                                     * 00001500

                                                                     * 00001600

          SRS  -  START RESET                                        * 00001700
          STT  -  START                                              * 00001800
          LDC  -  LOAD FROM CARDS                                    * 00001900
          LDT  -  LOAD FROM TAPE                                     * 00002000
          SSS  -  SET SENSE SWITCHES                                 * 00002100
          TAS  -  TAPE ASSIGNMENT                                    * 00002200
          CLR  -  CLEAR ALL 1401 CORE                                * 00002300
          DIS  -  DISPLAY 1401 CORE ON THE PRINTER                   * 00002400
          ALT  -  ALTER 1401 CORE                                    * 00002500
          WTM  -  WRITE TAPE MARK                                    * 00002600
          RWD  -  REWIND TAPE                                        * 00002700
          TRM  -  TERMINATE THE SIMULATOR                            * 00002800
                                                                     * 00002900
                                                                     * 00003000
                                                                     * 00003100

 16K BYTES ARE SET ASIDE FOR SIMULATED CORE, WITH EACH BYTE HAVING   * 00003200

 THE FOLOWING FORMAT.                                                * 00003300

     360 BIT        1401 BIT                                         * 00003400

        0            UNUSED                                          * 00003500

        1           WORD MARK                                        * 00003600

        2               B                                            * 00003700

        3               A                                            * 00003800

        4               8                                            * 00003900

        5               4                                            * 00004000

        6               2                                            * 00004100

        7               1                                            * 00004200

                                                                     * 00004300
                                                                     * 00004400

********************************************************************** 00004500
</pre>


enjoy!  

moshix. 
