    gem install whenever
    cd Backup
    mkdir config
    wheneverize
    cat config/schedule.rb
    
    every 1.day, at: '2:00 am' do
      command "backup perform -t full_backup"
    end

    whenever -f config/schedule.rb -w 'full backup'
    crontab -l
