######## Install CloudWatch Agent ############
Git clone first

sudo ./install.sh

######## Configure CloudWatch Agent ############
/opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-config-wizard

######## Start CloudWatch Agent ###############
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-ctl -a fetch-config -m ec2 -c file:configuration-file-path -s
