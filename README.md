ommands for the timer:
sudo cp /home/tkanell/repos/MagicMirrorE-Ink/magicmirror-eink.timer /etc/systemd/system/magicmirror-eink.timer

# 4. Reload systemd
sudo systemctl daemon-reload

# 5. Enable and start the timer (this will auto-start after reboot)
sudo systemctl enable magicmirror-eink.timer
sudo systemctl start magicmirror-eink.timer

# 6. Check timer status
sudo systemctl status magicmirror-eink.timer

# 7. Check when it will run next
sudo systemctl list-timers magicmirror-eink.timer
