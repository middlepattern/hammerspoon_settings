# hammerspoon_settings
my personal hammerspoon settings


hs.hotkey.bind({"cmd", "shift"}, "F", function()
    local app = hs.application.frontmostApplication()
    app:selectMenuItem({"Animation", "Keyframe Velocity..."})

    local win = hs.window.focusedWindow()
    local f = win:frame()

    if (f.h) > 300 then big_tab() else small_tab() end

  end)

  function big_tab()
    local delay = 200
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "9", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "9", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "9", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "9", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "return", delay)
  end

  function small_tab()
    local delay = 200
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "9", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "9", delay)
    hs.eventtap.keyStroke({}, "0", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "tab", delay)
    hs.eventtap.keyStroke({}, "return", delay)
  end
