# CBT314
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 314 is from Lionel Dyck in Austin, Texas and contains     *   FILE 314
//*           quite a few ISPF interface packages, and other        *   FILE 314
//*           stuff.                                                *   FILE 314
//*                                                                 *   FILE 314
//*           The member list probably more accurately reflects     *   FILE 314
//*           the contents of this file, than does the description  *   FILE 314
//*           of some details, below.  This file is constantly      *   FILE 314
//*           being revised.  For reference, please see Lionel's    *   FILE 314
//*           web site at:   http://github.com/lbdyck               *   FILE 314
//*                                                                 *   FILE 314
//*    Lionel Dyck's large collection of utilities has now been     *   FILE 314
//*    divided between Files 312, 313, 314, and 969.  All member    *   FILE 314
//*    names beginning with A-R are on File 312.  Names beginning   *   FILE 314
//*    with S-TS are on File 313.  Names from TX-Z are on File      *   FILE 314
//*    314.  File 969 contains the PDSEGEN ISPF application to      *   FILE 314
//*    exploit the capabilities of using PDSE Version 2 member      *   FILE 314
//*    generations.                                                 *   FILE 314
//*                                                                 *   FILE 314
//*    These four files contain quite a few separate utility        *   FILE 314
//*    packages which are unrelated to each other.  You can tell    *   FILE 314
//*    which members of these files belong to the same utility      *   FILE 314
//*    package, by the similarities in their member names.          *   FILE 314
//*                                                                 *   FILE 314
//*    Some utility packages will have several member names         *   FILE 314
//*    associated with them.  But these should all be similar       *   FILE 314
//*    to each other, letting you know that they belong to the      *   FILE 314
//*    same utility package.  You can see this, by looking at       *   FILE 314
//*    the member list shown below, so you can get the idea         *   FILE 314
//*    about how this packaging arrangement works.                  *   FILE 314
//*                                                                 *   FILE 314
//*    Documentation files which are in WORD format, or PDF         *   FILE 314
//*    format, have been included to make the use of the package    *   FILE 314
//*    associated with the doc, easier.  Usually a doc file in      *   FILE 314
//*    FB-80 EBCDIC text, has been included too.  To use the        *   FILE 314
//*    WORD or PDF format documentation, you have to download the   *   FILE 314
//*    member in BINARY to a PC, and look at the resulting file     *   FILE 314
//*    on the PC, using Microsoft WORD, or Adobe ACROBAT reader,    *   FILE 314
//*    respectively.                                                *   FILE 314
//*                                                                 *   FILE 314
//*       NAME       VER.MOD   LAST MODIFIED     SIZE   ID          *   FILE 314
//*       $DOC        01.03   2014/03/23 09:12     14 SBGOLOB       *   FILE 314
//*       TXT2CSV     01.00   2016/11/08 09:58    196 SYSLBD        *   FILE 314
//*       TXT2HTC$    03.04   2008/12/01 23:33     48 SBGOLOB       *   FILE 314
//*       TXT2HTML    03.04   2008/12/01 23:35   2924 SYSLBD        *   FILE 314
//*       TXT2PDF     04.02   2009/12/03 10:40  28935 SYSLBD        *   FILE 314
//*       TXT2PDF#    04.02   2009/12/03 10:42   6257 PDF           *   FILE 314
//*       TXT2PDF@    04.02   2009/12/03 10:42   5594 MSWORD        *   FILE 314
//*       TXT2PDFH    04.02   2009/12/03 10:38    305 SBGOLOB       *   FILE 314
//*       TXT2RTF     01.00   2016/11/08 01:21    669 SYSLBD        *   FILE 314
//*       TXT2RTF$    01.12   2010/07/21 08:07     79 SBGOLOB       *   FILE 314
//*       UIDLIST     01.01   2016/11/16 10:46     44 SYSLBD        *   FILE 314
//*       USSBATCH    01.00   2018/01/24 09:11    199 USS           *   FILE 314
//*       VB2FB       02.10   2017/10/11 10:54    942 LBD           *   FILE 314
//*       VCURSOR     01.14   2016/04/05 10:37    276 SYSLBD        *   FILE 314
//*       VCURSOR1    01.02   2016/04/01 13:43    227 OLD           *   FILE 314
//*       WHOSON      01.17   2025/03/20 07:47    573 WHOSON        *   FILE 314
//*       WORDNUM     01.02   2004/03/17 09:52     50 SYSLBD        *   FILE 314
//*       XIT         01.01   2004/05/02 10:24     28 SYSLBD        *   FILE 314
//*       XMIAFREN    05.68   2004/04/20 10:16     95 J-MLUCE       *   FILE 314
//*       XMITB64     01.00   2000/12/26 17:11    651 FELDMAN       *   FILE 314
//*       XMITFREN    05.68   2004/04/20 09:26     95 J-MLUCE       *   FILE 314
//*       XMITIHST    16.09   2016/11/07 09:32   3102 SBGOLOB       *   FILE 314
//*       XMITINS#    16.03   2016/04/03 18:01   2953 SYSLBD        *   FILE 314
//*       XMITINS@    16.03   2016/04/03 18:01   2938 SYSLBD        *   FILE 314
//*       XMITIP      16.19   2021/03/26 07:55  74266 XMITIP        *   FILE 314
//*       XMITIP$     01.01   2018/03/28 07:50   2058 TEXT          *   FILE 314
//*       XMITIP#     01.01   2018/03/28 07:49  13299 PDF           *   FILE 314
//*       XMITIP@     01.01   2018/03/28 07:49   5037 WORD          *   FILE 314
//*       XMITIPR     01.01   2018/03/28 07:49  13394 RTF           *   FILE 314
//*       XMITVM      01.00   2000/03/29 10:53    205 SYSLBD        *   FILE 314
//*       XMITXLAT    05.06   2004/03/19 14:55     69 PDF           *   FILE 314
//*       ZFSTOOLS    01.17   2025/03/17 11:40   3703 >7CHARS       *   FILE 314
//*       ZOOM        01.05   2016/04/04 07:15     30 SYSLBD        *   FILE 314
//*       ZOSLOG      01.00   2016/11/08 10:01    237 SYSLBD        *   FILE 314
//*       ZSTART      01.11   2017/12/18 05:54    817 LBD           *   FILE 314
//*       ZSYNC       05.01   2024/07/19 14:47   2019 ZSYNC         *   FILE 314
//*       ZTSOHELP    03.15   2023/10/01 12:29  12357 TSOHELP       *   FILE 314
//*                                                                 *   FILE 314
//*  Member TXT2CSV                                                 *   FILE 314
//*                                                                 *   FILE 314
//*     TXT2CSV is a very useful utility written in REXX            *   FILE 314
//*     and ISPF.  This is a rexx utility that will do a            *   FILE 314
//*     very basic conversion of a report ext file from             *   FILE 314
//*     plain text to a comma separated value format file           *   FILE 314
//*     which can then be processed using a workstation             *   FILE 314
//*     based spreadsheet or database tool.                         *   FILE 314
//*                                                                 *   FILE 314
//*  Member TXT2HTML                                                *   FILE 314
//*                                                                 *   FILE 314
//*     TXT2HTML is a REXX utility with an optional ISPF front      *   FILE 314
//*     end to convert your mainframe report file into a more       *   FILE 314
//*     usable HTML report.                                         *   FILE 314
//*                                                                 *   FILE 314
//*  Member TXT2PDF                                                 *   FILE 314
//*                                                                 *   FILE 314
//*     TXT2PDF is a great tool from Leland Lucius with an ISPF     *   FILE 314
//*     front-end by Lionel that will convert your mainframe        *   FILE 314
//*     report or data to a PDF with more options than you can      *   FILE 314
//*     count.                                                      *   FILE 314
//*                                                                 *   FILE 314
//*  Member TXT2RTF                                                 *   FILE 314
//*                                                                 *   FILE 314
//*     TXT2RTF is a REXX utility with an optional ISPF front-end   *   FILE 314
//*     that will convert your mainframe report into a file that    *   FILE 314
//*     can be opened using an word processor. Numerous formatting  *   FILE 314
//*     and control options are available.                          *   FILE 314
//*                                                                 *   FILE 314
//*  Member UIDLIST- This member is in TSO XMIT format.             *   FILE 314
//*                                                                 *   FILE 314
//*     List all Users and their UIDs by listing                    *   FILE 314
//*     the /u/userid directories                                   *   FILE 314
//*                                                                 *   FILE 314
//*  Member USSLIST                                                 *   FILE 314
//*                                                                 *   FILE 314
//*     Simple utility to invoke OMVS commands in batch.            *   FILE 314
//*     Easier than using BPXBATCH and other tools but may          *   FILE 314
//*     not provide everything for everyone.                        *   FILE 314
//*                                                                 *   FILE 314
//*  Member VB2FB - version 2.9 10/11/17                            *   FILE 314
//*                                                                 *   FILE 314
//*     Function:  Copy Fixed to Variable or Variable to Fixed      *   FILE 314
//*                                                                 *   FILE 314
//*                Tests the in dataset members to determine        *   FILE 314
//*                if there will be any data truncation before      *   FILE 314
//*                starting the copy operation.                     *   FILE 314
//*                                                                 *   FILE 314
//*     Syntax:    %vb2fb in out members ( options                  *   FILE 314
//*                                                                 *   FILE 314
//*                in        input dataset name                     *   FILE 314
//*                out       output dataset name                    *   FILE 314
//*                members   * for all                              *   FILE 314
//*                          member names                           *   FILE 314
//*                          member name pattern (e.g. abc*)        *   FILE 314
//*                (         required if options coded              *   FILE 314
//*                options   REPlace for replace                    *   FILE 314
//*                          TRunc   for truncation allow3ed        *   FILE 314
//*                          NORenum to bypass renumbering          *   FILE 314
//*                                                                 *   FILE 314
//*     Notes:                                                      *   FILE 314
//*               1. The ISPF Panels and Edit Macros that are       *   FILE 314
//*                  used by this exec are included inline below    *   FILE 314
//*                  and loaded dynamically using the LoadISPF      *   FILE 314
//*                  routine.                                       *   FILE 314
//*               2. If a member will be truncated during the       *   FILE 314
//*                  copy, and truncation has NOT been allowed,     *   FILE 314
//*                  then the member will be placed into ISPF       *   FILE 314
//*                  Edit and those records that may be             *   FILE 314
//*                  truncated will be displayed with all other     *   FILE 314
//*                  records hidden. (uses edit macro EMT)          *   FILE 314
//*               3. If the from member has ISPF sequence numbers   *   FILE 314
//*                  then the to member will be updated after the   *   FILE 314
//*                  copy to fix the sequence numbers (used edit    *   FILE 314
//*                  macros EM1 and EM2).                           *   FILE 314
//*                  - unless NORenum option is specified           *   FILE 314
//*                                                                 *   FILE 314
//*  Member VCURSOR                                                 *   FILE 314
//*                                                                 *   FILE 314
//*     VCURSOR is an updated version of Doug Nadel's VCURSOR that  *   FILE 314
//*     includes updates by Ken Tommiak and Lionel Dyck. Assign it  *   FILE 314
//*     to a PFK and then put the cursor on a DSN and it will       *   FILE 314
//*     opened that DSN in Browse, Edit, View, or the PDS command.  *   FILE 314
//*                                                                 *   FILE 314
//*  Member WHOSON (updated 11/21/2024)                             *   FILE 314
//*                                                                 *   FILE 314
//*     WHOSON uses SDSF REXX to find all logged on TSO and SSH     *   FILE 314
//*     users the SYSPLEX and display them for the user. Use with   *   FILE 314
//*     TSOTRAP (in file 313) to browse or view the results.        *   FILE 314
//*                                                                 *   FILE 314
//*     Added support to report on zOSMF (including zowe explorer)  *   FILE 314
//*     users on the system.                                        *   FILE 314
//*                                                                 *   FILE 314
//*     Now works under the OMVS shell if you prefer.               *   FILE 314
//*                                                                 *   FILE 314
//*  Member zFSTOOLS (updated 03/17/25)                             *   FILE 314
//*                                                                 *   FILE 314
//*     zFSTools is a collection of useful tools to work in the     *   FILE 314
//*     OMVS/USS environment - not solely with zfs files.           *   FILE 314
//*                                                                 *   FILE 314
//*     - Includes update from Patrick Loftus to add ZFSSHRK        *   FILE 314
//*       which is the zfsadm shrink option                         *   FILE 314
//*                                                                 *   FILE 314
//*  Member zSync    (updated 07/19/24)                             *   FILE 314
//*                                                                 *   FILE 314
//*     zSync is an ISPF application that will compare two          *   FILE 314
//*     PDS libraries (not load libraries) and present the user     *   FILE 314
//*     with a selection list of members with info on the delta.    *   FILE 314
//*     The user can then browse/edit members in both libraries,    *   FILE 314
//*     compare the members (using ispf edit or superc), exclude    *   FILE 314
//*     members in the table, and copy all eligible members from    *   FILE 314
//*     the from to the to PDS.                                     *   FILE 314
//*                                                                 *   FILE 314
//*     The comparison initially is based on ISPF Stats but         *   FILE 314
//*     an option is provided to use SuperC (CD or CS) to           *   FILE 314
//*     overtly check a member without stats if different.          *   FILE 314
//*                                                                 *   FILE 314
//*  Member ZSTART - Updated 12/12/17 Version 2.3                   *   FILE 314
//*                                                                 *   FILE 314
//*     ZSTART is an ISPF dialog to simplify managing the ISPF      *   FILE 314
//*     variable that controls what starts automatically when you   *   FILE 314
//*     enter ISPF.                                                 *   FILE 314
//*                                                                 *   FILE 314
//*     IBM has provided since z/OS 2.1 in ISPF the ability to      *   FILE 314
//*     define a set of ISPF commands to be invoked each time       *   FILE 314
//*     ISPF starts. This list is stored in the ISPF Profile        *   FILE 314
//*     Variable ZSTART under the ISR Profile.                      *   FILE 314
//*                                                                 *   FILE 314
//*     The format of the startup list is:                          *   FILE 314
//*                                                                 *   FILE 314
//*     1. Multiple commands on a line must be separated by         *   FILE 314
//*        a colon (;)                                              *   FILE 314
//*     2. TSO Commands must be prefixed by TSO                     *   FILE 314
//*        - the same as is required when manually invoked          *   FILE 314
//*          under ISPF                                             *   FILE 314
//*     3. ISPF commands require no prefix                          *   FILE 314
//*                                                                 *   FILE 314
//*     Sample:                                                     *   FILE 314
//*                                                                 *   FILE 314
//*             Start 3.4                                           *   FILE 314
//*             Start QW;Swap 1                                     *   FILE 314
//*                                                                 *   FILE 314
//*     This sample will create three ISPF screens. The first is    *   FILE 314
//*     the default ISPF Primary Options Menu, and then it will     *   FILE 314
//*     start a second session with ISPF 3.4. After starting the    *   FILE 314
//*     ISPF 3.4 display it will start a third session with MVS     *   FILE 314
//*     QuickRef and then Swap back to the first session.           *   FILE 314
//*                                                                 *   FILE 314
//*     The ZSTART commands may be viewed 1, 2, or 3 commands per   *   FILE 314
//*     row based on the setting for the Commands per Row in the    *   FILE 314
//*     upper right of the panel. If, when loading the rows, it is  *   FILE 314
//*     discovered that a row would exceed the characters allowed   *   FILE 314
//*     in the row, the Commands per Row will be changed from 1 to  *   FILE 314
//*     2 or from 2 to 3 as appropriate. The max commands per row   *   FILE 314
//*     is 3.                                                       *   FILE 314
//*                                                                 *   FILE 314
//*  Member ZTSOHELP - Updated 10/01/24 Version 3.15                *   FILE 314
//*                    ** In TSO XMIT format.                       *   FILE 314
//*                                                                 *   FILE 314
//*     Provide a list of all known TSO Help entries as             *   FILE 314
//*     defined within this exec. The exec is a self contained      *   FILE 314
//*     ISPF dialog with ISPF Message, ISPF Panels, and Edit        *   FILE 314
//*     macros that are dynamically loaded when needed.             *   FILE 314
//*                                                                 *   FILE 314
//*     The dialog presents the user with a list of TSO Help        *   FILE 314
//*     members that can then be selected for viewing in a          *   FILE 314
//*     formatted state.                                            *   FILE 314
//*                                                                 *   FILE 314
//*  Member ZOSLOG - This member is in TSO XMIT format.             *   FILE 314
//*                                                                 *   FILE 314
//*     The ZOSLOG ISPF Dialog found in this package will           *   FILE 314
//*     present the user with a list of all syslog log files        *   FILE 314
//*     in the z/OS system and allow the user to select a           *   FILE 314
//*     file to Browse, or View.                                    *   FILE 314
//*                                                                 *   FILE 314
//*     The only customization required is to verify/update         *   FILE 314
//*     the hlq for the syslog datasets variable in the exec        *   FILE 314
//*     and for the dataset name date.                              *   FILE 314
//*                                                                 *   FILE 314
//*  Member XMITIP - This member is in TSO XMIT format.             *   FILE 314
//*                  Updated 03/25/2021 - V20.03                    *   FILE 314
//*                                                                 *   FILE 314
//*     Distributing Reports from Batch Jobs via E-Mail             *   FILE 314
//*                                                                 *   FILE 314
//*     How many times have you wanted to have 'that' report in     *   FILE 314
//*     your e-mail inbox instead of having to wait for it to       *   FILE 314
//*     be printed and then delivered to you?                       *   FILE 314
//*                                                                 *   FILE 314
//*     This document describes a simple process that can be        *   FILE 314
//*     used by any batch job to distribute reports as e-mail       *   FILE 314
//*     attachments to electronic mail addresses.  You can          *   FILE 314
//*     distribute from one to n files to from one to n             *   FILE 314
//*     addresses.  The attachment will be translated from          *   FILE 314
//*     EBCDIC to ASCII during the electronic mail processing       *   FILE 314
//*     so only text files should be sent (note that special        *   FILE 314
//*     characters may not translate correctly so you should        *   FILE 314
//*     test your file before implementing this process into a      *   FILE 314
//*     production job).                                            *   FILE 314
//*                                                                 *   FILE 314
//*     The benefit is that you can send reports, using the         *   FILE 314
//*     REPORT keyword, as rich text format (rtf) documents and     *   FILE 314
//*     specify landscape or portrait orientation as well as        *   FILE 314
//*     the font size.  This approach is useful as the batch,       *   FILE 314
//*     formerly printed reports, arrive in the users mail box      *   FILE 314
//*     in a format similar to the printed report.                  *   FILE 314
//*                                                                 *   FILE 314
//*     Documentation for XMITIP is in three parts:                 *   FILE 314
//*                                                                 *   FILE 314
//*     Part 1 documents how to use the XMITIP REXX Application     *   FILE 314
//*            to electronically distribute messages and/or         *   FILE 314
//*            text files (as text attachments) to electronic       *   FILE 314
//*            mail addresses via the intranet or internet.         *   FILE 314
//*                                                                 *   FILE 314
//*     Part 2 documents how to view the attachment on the          *   FILE 314
//*            workstation.                                         *   FILE 314
//*                                                                 *   FILE 314
//*     Part 3 documents how to customize your own application      *   FILE 314
//*            to do this.                                          *   FILE 314
//*                                                                 *   FILE 314
//*     - - - - - - - - - - - - - - - - - - - - - - - - - - - -     *   FILE 314
//*                                                                 *   FILE 314
//*     Further documentation for XMITIP:                           *   FILE 314
//*                                                                 *   FILE 314
//*      This is a description of the XMITIP install partitioned    *   FILE 314
//*      dataset.  Approximate level is XMITIP 4.60 .               *   FILE 314
//*                                                                 *   FILE 314
//*      NOTE: A STEPLIB or update to linklist is now required      *   FILE 314
//*      to use this code.                                          *   FILE 314
//*                                                                 *   FILE 314
//*      Installation Step 1:                                       *   FILE 314
//*          To execute the RECEIVE member issue                    *   FILE 314
//*             "TSO EXEC 'hlq.pds-dsname(RECEIVE)' EXEC"           *   FILE 314
//*          This will create the rexx, panels, etc. libraries      *   FILE 314
//*          and place you in ISPF Browse on some key members.      *   FILE 314
//*      Installation Step 2.                                       *   FILE 314
//*          Update XMITIPCU - see the Installation Guide.          *   FILE 314
//*                                                                 *   FILE 314
//*      Updates can be found at http://github.com/lbdyck           *   FILE 314
//*                                                                 *   FILE 314
//*      Mutual Support:                                            *   FILE 314
//*      Mark Regan has created a listserv for mutual support:      *   FILE 314
//*                                                                 *   FILE 314
//*         Subscribe:    xmitip-subscribe@yahoogroups.com          *   FILE 314
//*         Unsubscribe:  xmitip-unsubscribe@yahoogroups.com        *   FILE 314
//*         Post message: xmitip@yahoogroups.com                    *   FILE 314
//*         List owner:   xmitip-owner@yahoogroups.com              *   FILE 314
//*                                                                 *   FILE 314
//*      XMITIP will work with both the older SMTP and newer        *   FILE 314
//*      CSSMTP servers on z/OS.                                    *   FILE 314
//*                                                                 *   FILE 314
//*      Caution: Be sure to run the IVPJOB to verify your          *   FILE 314
//*      installation.                                              *   FILE 314
//*                                                                 *   FILE 314
//*      $DOC     what you are reading                              *   FILE 314
//*      $WISH    list of requested changes/enhancements            *   FILE 314
//*      ALLOCGDG doc on using this new exec                        *   FILE 314
//*      ASM      Assembler source modules                          *   FILE 314
//*               * in IDTF format                                  *   FILE 314
//*      CHANGES  what's changed                                    *   FILE 314
//*      COMPILE  information if you want to compile this           *   FILE 314
//*               application                                       *   FILE 314
//*      DISTINFO information on using distribution lists           *   FILE 314
//*      EXEC     The rexx execs in TSO Transmit (IDTF) format      *   FILE 314
//*      FEEDBACK Sample JCL you can use to send feedback on XMITIP *   FILE 314
//*      IEFDB401 Sample dynamic allocation exit from University    *   FILE 314
//*               of Florida modified by Lionel Dyck.  Will         *   FILE 314
//*               issue Notify messages to TSO users for            *   FILE 314
//*               incoming mail.                                    *   FILE 314
//*      IOF      Shows how to e-mail from IOF using XMITSDSF       *   FILE 314
//*      IVP*     These members are the Installation                *   FILE 314
//*               Verification members - see member IVPJOB for      *   FILE 314
//*               the job to run                                    *   FILE 314
//*      LDAP     Information on the setup for using LDAP to        *   FILE 314
//*               query/validate e-mail addresses                   *   FILE 314
//*      LICENSE  The license under which this package is           *   FILE 314
//*               distributed                                       *   FILE 314
//*      LOAD     Load library containing various load modules      *   FILE 314
//*               * in IDTF format                                  *   FILE 314
//*      MSGS     The ISPF messages in TSO Transmit (IDTF) format   *   FILE 314
//*      NOTIFY   From Paul Wells: (in TSO Transmit (IDTF)          *   FILE 314
//*               format) This allows you to route the SMTP         *   FILE 314
//*               Logfile to OPS/MVS which will then process the    *   FILE 314
//*               logfile and issue messages to the user about      *   FILE 314
//*               incoming mail.                                    *   FILE 314
//*      PQ*****  APARs that you might find interesting  <<<<<<<<   *   FILE 314
//*      PANELS   The ISPF panels in TSO Transmit (IDTF) format     *   FILE 314
//*      PDF      Short description on how to use XMITIPPD          *   FILE 314
//*               outside of XMITIP to create PDF files.            *   FILE 314
//*      RECEIVE  A simple exec to receive the EXEC and PANELS      *   FILE 314
//*               members into partitioned datasets                 *   FILE 314
//*      SAMPDISC Sample Disclaimers if you need to use one         *   FILE 314
//*      SDSF     Information on using the XMITSDSF to interface    *   FILE 314
//*               to XMITIPFE                                       *   FILE 314
//*      SMTPRTN  Batch JCL for REXX Code SMTPRTN                   *   FILE 314
//*      SMTPVFY  Batch JCL to verify that SMTP is properly         *   FILE 314
//*               installed                                         *   FILE 314
//*      SPOOF1   Discussion on spoofing and the XMITIP             *   FILE 314
//*               antispoof option                                  *   FILE 314
//*      SPOOF2   A technique to prevent spoofing using SECURE      *   FILE 314
//*               SMTP * Thanks to Matt                             *   FILE 314
//*      TCPDATA  Information on how TCP/IP looks for the           *   FILE 314
//*               TCPDATA file                                      *   FILE 314
//*      TEST$GIF Sample GIF for testing GIF attachments            *   FILE 314
//*               (US Flag)                                         *   FILE 314
//*      TEST$CSV Sample CSV for testing CSV attachments            *   FILE 314
//*      TESTXMIT Rexx code to test the new dialog using altlib     *   FILE 314
//*               and libdef ** May also be used under a            *   FILE 314
//*               different name to invoke XMITIP ** without        *   FILE 314
//*               copying the xmitip libraries into production      *   FILE 314
//*               libraries                                         *   FILE 314
//*      TMSGQ    Sample exec for testing MSGQ                      *   FILE 314
//*      TXT2HTML User documentation on Text-to-HTML tool           *   FILE 314
//*      TOOLS    Brief summary of the tools included with XMITIP   *   FILE 314
//*      XMITSTAT Doc on how to generate SMTP Statistics            *   FILE 314
//*      STATJCL  JCL to generate SMTP statistics from the IBM      *   FILE 314
//*               SMTP Server.                                      *   FILE 314
//*                                                                 *   FILE 314
//*      For National Language Support:                             *   FILE 314
//*                                                                 *   FILE 314
//*      PDFXLTB  Build a national language translate table for     *   FILE 314
//*               XMITIPTR *                                        *   FILE 314
//*      SMTPXLTB Build a national language translate table for     *   FILE 314
//*               SMTP *                                            *   FILE 314
//*      PQ36249  Documents IBM APAR for @ support for other        *   FILE 314
//*               languages                                         *   FILE 314
//*      FRENCH   Information on setting up the SMTP translation    *   FILE 314
//*               tables for the French language.  * thanks to      *   FILE 314
//*               Felipe Cvitanich                                  *   FILE 314
//*                                                                 *   FILE 314
//*      For Disclaimer support:                                    *   FILE 314
//*                                                                 *   FILE 314
//*      Update XMITIPCU variable with the fully qualified data     *   FILE 314
//*      set name of a data set which contains your                 *   FILE 314
//*      installation's standard disclaimer.  The contents of       *   FILE 314
//*      this data set will be included with every e-mail for       *   FILE 314
//*      which a message is generated.                              *   FILE 314
//*                                                                 *   FILE 314
//*      IMPORTANT: Local customizations should be made in the      *   FILE 314
//*      XMITIPCU rexx exec and in the XMITLDAP rexx exec:          *   FILE 314
//*                                                                 *   FILE 314
//*        XMITIPCU - general customizations                        *   FILE 314
//*        XMITLDAP - customizations related to the use of ldap     *   FILE 314
//*                   to verify and/or find e-mail addresses.       *   FILE 314
//*        XMITIPML - you may need to customize this exec if the    *   FILE 314
//*                   ldap server returns information in a          *   FILE 314
//*                   format different from what is defined. (if    *   FILE 314
//*                   you change this you should remember what      *   FILE 314
//*                   you changed for future updates and if you     *   FILE 314
//*                   can generalize what you've done let me        *   FILE 314
//*                   know).  PLUS you may need to change the       *   FILE 314
//*                   comments on the panel XMITIPML.               *   FILE 314
//*                                                                 *   FILE 314
//*      If you need to change the dollar symbol to a pound or      *   FILE 314
//*      you need to change the PDF ebcdic->ascii translation       *   FILE 314
//*      table then you need to update XMITIPTR.                    *   FILE 314
//*                                                                 *   FILE 314
//*         e.g. For the dollar to pound change location 5B to      *   FILE 314
//*              be A3                                              *   FILE 314
//*                                                                 *   FILE 314
//*      ZIP Notes:                                                 *   FILE 314
//*                                                                 *   FILE 314
//*      1. PKZIP/MVS can be found at www.asizip.com                *   FILE 314
//*      2. ISPZIP can be found at www.ase.com.au                   *   FILE 314
//*      3. ZIP390 can be found at www.data21.com                   *   FILE 314
//*      4. InfoZip is now supported                                *   FILE 314
//*         InfoZIp can be found (for FREE) at:                     *   FILE 314
//*           ftp://ftp.freesoftware.com/pub/infozip/MVS/           *   FILE 314
//*         - an alternate (newer) download from                    *   FILE 314
//*           http://www.mildredbrennan.com/blog/?p=309             *   FILE 314
//*         - does not support name-in-archive for pds members      *   FILE 314
//*         - infozip must be installed in a steplib or in          *   FILE 314
//*           linklist ****                                         *   FILE 314
//*         - load module (zip) is provided in the load library     *   FILE 314
//*         - you may need to download and recompile InfoZip if     *   FILE 314
//*           you need a different ASCII character set.             *   FILE 314
//*      5. PKZIP/MVS pre 2.51 does not support the                 *   FILE 314
//*         name-in-archive option                                  *   FILE 314
//*      6. PKZIP/MVS version 5 has a problem with mixed case       *   FILE 314
//*         commands XMITIP has been fixed to generate upper        *   FILE 314
//*         case commands for PKZIP/MVS V5.  Now it seems that      *   FILE 314
//*         ASI has a patch to allow mixed case - available at      *   FILE 314
//*         their web site.                                         *   FILE 314
//*      7. PKZIP/MVS Version 5 requires fix level 508 at a         *   FILE 314
//*         minimum                                                 *   FILE 314
//*      8. ISPZIP issues                                           *   FILE 314
//*         - does not support ZIPPASS or ZIPMETHOD                 *   FILE 314
//*         - does not support name-in-archive for pds members      *   FILE 314
//*         - resultant zip file does not work with Infozip         *   FILE 314
//*           or Lotus Notes Viewer                                 *   FILE 314
//*                                                                 *   FILE 314
//*      National Language Information:                             *   FILE 314
//*      If you have an issue with your language and the @          *   FILE 314
//*      character then check out IBM APAR PQ36249                  *   FILE 314
//*                                                                 *   FILE 314
//*      Comments, suggestions, and complaints should be            *   FILE 314
//*      directed to the author at:                                 *   FILE 314
//*                                                                 *   FILE 314
//*      Lionel B. Dyck                                             *   FILE 314
//*      email:   lbdyck@gmail.com                                  *   FILE 314
//*      github:  github.com/lbdyck                                 *   FILE 314
//*                                                                 *   FILE 314
```
