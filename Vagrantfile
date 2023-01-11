Vagrant.configure('2') do |config|
    config.vm.box = 'StefanScherer/windows_2022'

    config.vm.define 'windows'

    # Prevent SharedFoldersEnableSymlinksCreate errors
    config.vm.synced_folder '.', '/vagrant', disabled: true
end
