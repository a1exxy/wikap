#!/usr/bin/perl -w

use ExtUtils::Installed;

$installed = ExtUtils::Installed->new ();

foreach $module ($installed->modules ()){

printf "Module: %s\t\tVersion: %s\n", $module, $installed->version ($module);

}