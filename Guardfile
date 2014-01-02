coffescript_command = "coffee -cbj public/js/app.js src/coffeescript/"
system coffescript_command # guard:process doesn't run at start

guard :copy, from: "src/img", to: "public/img", run_at_start: true, mkpath: true

guard :process, name: "coffeescript", command: coffescript_command do
  watch %r{^src/coffeescript}
end

guard :haml, input: "src/haml", output: "public", run_at_start: true

guard :sass, input: "src/scss", output: "public/css", all_on_start: true

guard :livereload do
  watch %r{^public}
end

notification :growl
