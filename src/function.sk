Options:
	prefix: &8&l(&c!&8&l)
	cooldown.message: &cMasih cooldown!

function romanNumeral(n: integer) :: string:
    set {_r::*} to "M", "CM", "D", "CD", "C", "XC", "L", "XL", "X", "IX", "V", "IV" and "I"
    set {_v::*} to 1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4 and 1
    set {_o} to ""
    loop {_v::*}:
        loop floor({_n} / loop-value) times:
            set {_o} to "%{_o}%%{_r::%loop-index-1%}%"
            subtract loop-value-1 from {_n}
    return {_o}

function GetSimpleValueYaml(p: offline player, path: text, location: text) :: object:
	if yaml "%{_location}%" is not loaded:
		load yaml "%{_location}%" as "%{_location}%"
	set {_value} to yaml value "%{_path}%" from "%{_location}%"
	return {_value}

function GetSimpleLoopValueYaml(p: offline player, path: text, location: text) :: objects:
	if yaml "%{_location}%" is not loaded:
		load yaml "%{_location}%" as "%{_location}%"
	set {_value::*} to colored yaml list "%{_path}%" from "%{_location}%"
	return {_value::*}

function SaveSimpleValueYaml(p: offline player, path: text, location: text, value: object):
	if yaml "%{_location}%" is not loaded:
		load yaml "%{_location}%" as "%{_location}%"
	if {_value} is number:
		set {_value} to floor({_value})
	send "%{_value}%" to console
	set yaml value "%{_path}%" from "%{_location}%" to {_value}
	save "%{_location}%"

function Guiborder_chest(p: player, type: text):
	play sound "entity.horse.armor" with volume 1 to {_p}
	loop integers between 0 and menu size of {_p}'s current inventory - 1:
		format gui slot loop-number of {_p} with black stained glass pane named "&7Panel" 
	if {_type} is "3row":
		format gui slot 0 of {_p} with iron bars named "&7Panel"
		format gui slot 1 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 3 of {_p} with iron bars named "&7Panel"
		format gui slot 4 of {_p} with iron bars named "&7Panel"
		format gui slot 5 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 7 of {_p} with iron bars named "&7Panel"
		format gui slot 9 of {_p} with iron bars named "&7Panel"
		format gui slot 17 of {_p} with iron bars named "&7Panel"
		format gui slot 18 of {_p} with iron bars named "&7Panel"
		format gui slot 19 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 21 of {_p} with iron bars named "&7Panel"
		format gui slot 22 of {_p} with iron bars named "&7Panel"
		format gui slot 23 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 25 of {_p} with iron bars named "&7Panel"
		format gui slot 26 of {_p} with iron bars named "&7Panel"
	else if {_type} is "4row":
		format gui slot 0 of {_p} with iron bars named "&7Panel"
		format gui slot 1 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 3 of {_p} with iron bars named "&7Panel"
		format gui slot 4 of {_p} with iron bars named "&7Panel"
		format gui slot 5 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 7 of {_p} with iron bars named "&7Panel"
		format gui slot 9 of {_p} with iron bars named "&7Panel"
		format gui slot 17 of {_p} with iron bars named "&7Panel"
		format gui slot 18 of {_p} with iron bars named "&7Panel"
		format gui slot 26 of {_p} with iron bars named "&7Panel"
		format gui slot 27 of {_p} with iron bars named "&7Panel"
		format gui slot 28 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 30 of {_p} with iron bars named "&7Panel"
		format gui slot 31 of {_p} with iron bars named "&7Panel"
		format gui slot 32 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 34 of {_p} with iron bars named "&7Panel"
		format gui slot 35 of {_p} with iron bars named "&7Panel"
	else if {_type} is "5row":
		format gui slot 0 of {_p} with iron bars named "&7Panel"
		format gui slot 1 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 3 of {_p} with iron bars named "&7Panel"
		format gui slot 4 of {_p} with iron bars named "&7Panel"
		format gui slot 5 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 7 of {_p} with iron bars named "&7Panel"
		format gui slot 9 of {_p} with iron bars named "&7Panel"
		format gui slot 17 of {_p} with iron bars named "&7Panel"
		format gui slot 27 of {_p} with iron bars named "&7Panel"
		format gui slot 35 of {_p} with iron bars named "&7Panel"
		format gui slot 36 of {_p} with iron bars named "&7Panel"
		format gui slot 37 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 39 of {_p} with iron bars named "&7Panel"
		format gui slot 40 of {_p} with iron bars named "&7Panel"
		format gui slot 41 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 43 of {_p} with iron bars named "&7Panel"
		format gui slot 44 of {_p} with iron bars named "&7Panel"
	else if {_type} is "6row":
		format gui slot 0 of {_p} with iron bars named "&7Panel"
		format gui slot 1 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 3 of {_p} with iron bars named "&7Panel"
		format gui slot 4 of {_p} with iron bars named "&7Panel"
		format gui slot 5 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 7 of {_p} with iron bars named "&7Panel"
		format gui slot 9 of {_p} with iron bars named "&7Panel"
		format gui slot 17 of {_p} with iron bars named "&7Panel"
		format gui slot 36 of {_p} with iron bars named "&7Panel"
		format gui slot 44 of {_p} with iron bars named "&7Panel"
		format gui slot 45 of {_p} with iron bars named "&7Panel"
		format gui slot 46 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 48 of {_p} with iron bars named "&7Panel"
		format gui slot 49 of {_p} with iron bars named "&7Panel"
		format gui slot 50 of {_p} with iron bars named "&7Panel"
		#
		format gui slot 52 of {_p} with iron bars named "&7Panel"
		format gui slot 53 of {_p} with iron bars named "&7Panel"
	else:
		send "&cBorder GUI yang di set sepertinya belum di buat? ada di file serbaguna" to {_p} 

function Toggle_alias(value: boolean) :: text:
	if {_value} is true:
		return "&aAktif"
	else if {_value} is false:
		return "&cNonaktif"
	else:
		return "&d%{_value}%"

function Numberformat(integer: object) :: text:
	if {_integer} is number:
		set {_integer} to floor({_integer})
	set {_integer} to "%{_integer}%"
	return regex replace "(?<=\d)(?=(\d\d\d)+(?!\d))" with "." in {_integer}
	  
function Logmessage(message: text):
	set {_p} to "Low_Scarlet" parsed as offline player
	send "[SKRIPT-DEBUG][LOG] %{_message}%." to console

function Errormessage_guide(p: player):
	send "{@prefix} &7&oScreenshot semua message ini ke Owner atau ke Channel ##Semua-Laporan di Group Discord server!" to {_p}
	Logmessage("%{_p}% Menemukan Bug/Error!")

function Cooldown_CountDown(lasttriger: date, cooldown: timespan, type: number) :: text:
	set {_CD} to difference between {_lasttriger} and now
	set {_TargetTime} to {_lasttriger}
	add {_cooldown} to {_TargetTime}
	set {_CD2} to difference between {_TargetTime} and now
	#
	set {_split::*} to split "%{_CD2}%" at " "
	set {_split::4} to {_split::4} parsed as number
	set {_split::4} to floor({_split::4})
	if {_type} is 1:
		set {_cdformat} to "&a%{_split::1}% %{_split::2}%"
	else if {_type} is 2:
		if {_split::4} is set:
			set {_cdformat} to "&a%{_split::1}% %{_split::2}%, %{_split::4}% %{_split::5}%"
		else:
			Cooldown_CountDown({_lasttriger}, {_cooldown}, 1)
	#
	replace all "seconds" with "Detik" in {_cdformat}
	replace all "minutes" with "Menit" in {_cdformat}
	replace all "hours" with "Jam" in {_cdformat}
	replace all "days" with "Hari" in {_cdformat}
	#
	return {_cdformat}
	
	
