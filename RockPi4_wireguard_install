show_temp(){
tz0=$(</sys/class/thermal/thermal_zone0/temp)
tz1=$(</sys/class/thermal/thermal_zone1/temp)
echo -e "Temperature now is: \e[100m$((tz0/1000))°C $((tz1/1000))°C\e[49m"
}

echo $(show_temp)
apt-get -y update
echo $(show_temp)
apt-get -y upgrade
echo $(show_temp)

version=$(uname -r)
if [[ "${version}" == *"rockchip64"* ]]; then
echo -e "\e[100mLet's move on.\e[49m"
apt-get install linux-headers-current-rockchip64
echo ""
echo $(show_temp)
echo ""
echo -e "\e[100mHave a nice day!\e[49m"
echo ""
else
echo -e "\e[101mSomething went wrong with the Kernel-headers! Please check it.\e[49m"
echo -e "\e[101mYour installed Kernel is ${version} but this installer is forthe Rockchip64 one.\e[49m"
echo -e "\e[101mThis script was made 02.07.2020. If you have an RockPi4 and this does not work-\e[49m"
echo -e "\e[101m maby this installer is to old..\e[49m"
echo $(show_temp)
fi
