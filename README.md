# Hex Records TextMate Bundle README

# Installation

Install by double clicking.

# General

* [Intel Hex File Format](http://srecord.sourceforge.net/man/man5/srec_intel.html) - _Description of the file format_

A hex file consists of records that match the following regular expressions:

Data Record
^:(\h{2})(\h{4})(00)(\h{2,510})(\h{2})$

End of File Record
^:00000001[fF][fF]$

Extended Linear Address Record, Extended Segment Address Record
^:020000(0[24])(\h{4})(\h{2})$

Start Linear Address Record, Start Segment Address Record
^:040000(0[35])(\h{8})(\h{2})$

The bundle attempts to assign reasonable colors and allows for folding the data sections.