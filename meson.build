project('Qogir', version: '2023-02-27')

if get_option('tweaks').length() > 0
	tweaks = true
	sassc = find_program('sassc', required: true)
	sassc_opts = ['-M', '-t', 'expanded']
endif

env = environment()
env.set('DESTDIR', get_option('datadir')/'themes')

subdir('src')
