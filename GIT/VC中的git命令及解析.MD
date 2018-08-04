
# VC中的git命令及解析

  // 控制已更新文件的自动保存。接受的值:“off”、"afterDelay”、“onFocusChange”(编辑器失去焦点)、“onWindowChange”(窗口失去焦点)。如果设置为“afterDelay”，则可在 "files.autoSaveDelay" 中配置延迟。
  "files.autoSave": "off",

  // 以像素为单位控制字号。
  "editor.fontSize": 14,

  // 控制字体系列。
  "editor.fontFamily": "Consolas, 'Courier New', monospace",

  // 一个制表符等于的空格数。该设置在 "editor.detectIndentation" 启用时根据文件内容可能会被覆盖。
  "editor.tabSize": 4,

  // 控制编辑器在空白字符上显示特殊符号的方式。可选值为 "none"(无)、"boundary"(边界) 或 "all"(所有)。选择 "boundary" 选项，则不会在单词之间的单个空格上显示特殊符号。
  "editor.renderWhitespace": "none",

  // 控制光标样式，接受的值为 "block"、"block-outline"、"line"、"line-thin" 、"underline" 和 "underline-thin"
  "editor.cursorStyle": "line",

  // 在通过鼠标添加多个光标时使用的修改键。"ctrlCmd" 会映射为 "Ctrl" (Windows 和 Linux) 或 "Command" (macOS)。“转到定义”和“打开链接”功能所需的鼠标动作将会相应调整，不与多光标修改键冲突。
  "editor.multiCursorModifier": "alt",

  // 按 Tab 键时插入空格。该设置在 "editor.detectIndentation" 启用时根据文件内容可能会被覆盖。
  "editor.insertSpaces": true,

  // 控制折行方式。可以选择： - “off” （禁用折行）， - “on” （视区折行）， - “wordWrapColumn”（在“editor.wordWrapColumn”处折行）或 - “bounded”（在视区与“editor.wordWrapColumn”两者的较小者处折行）。
  "editor.wordWrap": "off",

  // 配置 glob 模式以在搜索中排除文件和文件夹。例如，文件资源管理器根据此设置决定文件或文件夹的显示和隐藏。
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true
  },

  // 配置语言的文件关联(如: "*.extension": "html")。这些关联的优先级高于已安装语言的默认关联。
  "files.associations": {}

}
,
{


  // 控制差异编辑器是否将对前导空格或尾随空格的更改显示为差异
  "diffEditor.ignoreTrimWhitespace": true,

  // 控制差异编辑器是否为已添加/删除的更改显示 +/- 指示符号
  "diffEditor.renderIndicators": true,

  // 控制 Diff 编辑器以并排或内联形式显示差异
  "diffEditor.renderSideBySide": true,

  // 控制是否应在遇到提交字符时接受建议。例如，在 JavaScript 中，分号(";")可以为提交字符，可接受建议并键入该字符。
  "editor.acceptSuggestionOnCommitCharacter": true,

  // 控制按“Enter”键是否像按“Tab”键一样接受建议。这能帮助避免“插入新行”和“接受建议”之间的歧义。值为“smart”时表示，仅当文字改变时，按“Enter”键才能接受建议
  "editor.acceptSuggestionOnEnter": "on",

  // 控制编辑器是否应运行在对屏幕阅读器进行优化的模式。
  "editor.accessibilitySupport": "auto",

  // 控制编辑器是否应该在左括号后自动插入右括号
  "editor.autoClosingBrackets": true,

  // 控制编辑器是否在用户键入、粘贴或移动行时自动调整缩进。语言的缩进规则必须可用。
  "editor.autoIndent": true,

  // 控制编辑器是否显示 CodeLens
  "editor.codeLens": true,

  // 控制编辑器是否显示内联颜色修饰器和颜色选取器。
  "editor.colorDecorators": true,

  // 控制光标动画样式，可能的值为 "blink"、"smooth"、"phase"、"expand" 和 "solid"
  "editor.cursorBlinking": "blink",

  // 控制光标样式，接受的值为 "block"、"block-outline"、"line"、"line-thin" 、"underline" 和 "underline-thin"
  "editor.cursorStyle": "line",

  // 当 editor.cursorStyle 设置为 "line" 时控制光标的宽度。
  "editor.cursorWidth": 0,

  // 当打开文件时，将基于文件内容检测 "editor.tabSize" 和 "editor.insertSpaces"。
  "editor.detectIndentation": true,

  // 控制编辑器是否应该允许通过拖放移动所选项。
  "editor.dragAndDrop": true,

  // 控制没有选择内容的复制是否复制当前行。
  "editor.emptySelectionClipboard": true,

  // 控制当编辑器中选中多个字符或多行文字时是否开启“在选定内容中查找”选项 
  "editor.find.autoFindInSelection": false,

  // 控制是否将编辑器的选中内容作为搜索词填入到查找组件
  "editor.find.seedSearchStringFromSelection": true,

  // 控制编辑器是否启用代码折叠功能
  "editor.folding": true,

  // 控制字体系列。
  "editor.fontFamily": "Consolas, 'Courier New', monospace",

  // 启用字体连字
  "editor.fontLigatures": false,

  // 以像素为单位控制字号。
  "editor.fontSize": 14,

  // 控制字体粗细。
  "editor.fontWeight": "normal",

  // 控制编辑器是否应自动设置粘贴内容的格式。格式化程序必须可用并且能设置文档中某一范围的格式。
  "editor.formatOnPaste": false,

  // 保存时设置文件的格式。格式化程序必须可用，不能自动保存文件，并且不能关闭编辑器。
  "editor.formatOnSave": false,

  // 控制编辑器是否应在键入后自动设置行的格式
  "editor.formatOnType": false,

  // 控制编辑器是否应呈现垂直字形边距。字形边距最常用于调试。
  "editor.glyphMargin": true,

  // 控制光标是否应隐藏在概述标尺中。
  "editor.hideCursorInOverviewRuler": false,

  // 按 Tab 键时插入空格。该设置在 "editor.detectIndentation" 启用时根据文件内容可能会被覆盖。
  "editor.insertSpaces": true,

  // 以像素为单位控制字符间距。
  "editor.letterSpacing": 0,

  // 启用代码操作小灯泡提示
  "editor.lightbulb.enabled": true,

  // 控制行高。使用 0 通过字号计算行高。
  "editor.lineHeight": 0,

  // 控制行号的显示。可选值为 "on"、"off"、"relative" 和 "interval"。
  "editor.lineNumbers": "on",

  // 控制编辑器是否应检测链接并使它们可被点击
  "editor.links": true,

  // 当选择其中一项时，将突出显示匹配的括号。
  "editor.matchBrackets": true,

  // 控制是否显示 minimap
  "editor.minimap.enabled": true,

  // 限制最小映射的宽度，尽量多地呈现特定数量的列
  "editor.minimap.maxColumn": 120,

  // 呈现某行上的实际字符(与颜色块相反)
  "editor.minimap.renderCharacters": true,

  // 控制是否自动隐藏小地图滑块。可选值为 "always" 和 "mouseover"
  "editor.minimap.showSlider": "mouseover",

  // 控制在哪一侧显示小地图。可选值为 "right" (右) 和 "left" (左)
  "editor.minimap.side": "right",

  // 要对鼠标滚轮滚动事件的 "deltaX" 和 "deltaY" 使用的乘数 
  "editor.mouseWheelScrollSensitivity": 1,

  // 通过使用鼠标滚轮同时按住 Ctrl 可缩放编辑器的字体
  "editor.mouseWheelZoom": false,

  // 在通过鼠标添加多个光标时使用的修改键。"ctrlCmd" 会映射为 "Ctrl" (Windows 和 Linux) 或 "Command" (macOS)。“转到定义”和“打开链接”功能所需的鼠标动作将会相应调整，不与多光标修改键冲突。
  "editor.multiCursorModifier": "alt",

  // 控制编辑器是否应该突出显示语义符号次数
  "editor.occurrencesHighlight": true,

  // 控制概述标尺周围是否要绘制边框。
  "editor.overviewRulerBorder": true,

  // 控制可在概述标尺同一位置显示的效果数量
  "editor.overviewRulerLanes": 3,

  // 启用在输入时显示含有参数文档和类型信息的小面板
  "editor.parameterHints": true,

  // 控制键入时是否应自动显示建议
  "editor.quickSuggestions": {
    "other": true,
    "comments": false,
    "strings": false
  },

  // 控制延迟多少毫秒后将显示快速建议
  "editor.quickSuggestionsDelay": 10,

  // 控制编辑器是否应呈现控制字符
  "editor.renderControlCharacters": false,

  // 控制编辑器是否应呈现缩进参考线
  "editor.renderIndentGuides": true,

  // 控制编辑器应如何呈现当前行突出显示，可能为“无”、“装订线”、“线”和“全部”。
  "editor.renderLineHighlight": "line",

  // 控制编辑器在空白字符上显示特殊符号的方式。可选值为 "none"(无)、"boundary"(边界) 或 "all"(所有)。选择 "boundary" 选项，则不会在单词之间的单个空格上显示特殊符号。
  "editor.renderWhitespace": "none",

  // 控制选取范围是否有圆角
  "editor.roundedSelection": true,

  // 在一定数量的等宽字符后显示垂直标尺。输入多个值，显示多个标尺。若数组为空，则不绘制标尺。
  "editor.rulers": [],

  // 控制编辑器是否可以滚动到最后一行之后
  "editor.scrollBeyondLastLine": true,

  // 控制编辑器是否应突出显示选项的近似匹配
  "editor.selectionHighlight": true,

  // 控制是否自动隐藏导航线上的折叠控件。
  "editor.showFoldingControls": "mouseover",

  // 控制编辑器是否在滚动时使用动画
  "editor.smoothScrolling": false,

  // 控制是否将代码段与其他建议一起显示以及它们的排序方式。
  "editor.snippetSuggestions": "inline",

  // 即使在双击编辑器内容或按 Esc 键时，也要保持速览编辑器的打开状态。
  "editor.stablePeek": false,

  // 建议小组件的字号
  "editor.suggestFontSize": 0,

  // 建议小组件的行高
  "editor.suggestLineHeight": 0,

  // 控制键入触发器字符时是否应自动显示建议
  "editor.suggestOnTriggerCharacters": true,

  // 控制在建议列表中如何预先选择建议。
  "editor.suggestSelection": "recentlyUsed",

  // 当其前缀匹配时插入代码段。当 "quickSuggestions" 未启用时，效果最佳。
  "editor.tabCompletion": false,

  // 一个制表符等于的空格数。该设置在 "editor.detectIndentation" 启用时根据文件内容可能会被覆盖。
  "editor.tabSize": 4,

  // 覆盖当前所选颜色主题中的编辑器颜色和字体样式。
  "editor.tokenColorCustomizations": {},

  // 删除尾随自动插入的空格
  "editor.trimAutoWhitespace": true,

  // 在制表位后插入和删除空格
  "editor.useTabStops": true,

  // 控制是否根据文档中的文字计算自动完成列表。
  "editor.wordBasedSuggestions": true,

  // 执行文字相关的导航或操作时将用作文字分隔符的字符
  "editor.wordSeparators": "`~!@#$%^&*()-=+[{]}\\|;:'\",.<>/?",

  // 控制折行方式。可以选择： - “off” （禁用折行）， - “on” （视区折行）， - “wordWrapColumn”（在“editor.wordWrapColumn”处折行）或 - “bounded”（在视区与“editor.wordWrapColumn”两者的较小者处折行）。
  "editor.wordWrap": "off",

  // 在 "editor.wordWrap" 为 "wordWrapColumn" 或 "bounded" 时控制编辑器列的换行。
  "editor.wordWrapColumn": 80,

  // 控制折行的缩进。可以是“none”、“same”或“indent”。
  "editor.wrappingIndent": "same"

}
,
{


  // 是否总是显示源代码管理提供程序部分。
  "scm.alwaysShowProviders": false,

  // 控制编辑器中差异的显示效果。
  "scm.diffDecorations": "all"

}
,
{


  // 控制工作台中活动栏的可见性。
  "workbench.activityBar.visible": true,

  // 覆盖当前所选颜色主题的颜色。
  "workbench.colorCustomizations": {},

  // 指定工作台中使用的颜色主题。
  "workbench.colorTheme": "Default Dark+",

  // 控制命令面板中保留最近使用命令的数量。设置为 0 时禁用命令历史功能。
  "workbench.commandPalette.history": 50,

  // 控制是否在再次打开命令面板时恢复上一次的输入内容。
  "workbench.commandPalette.preserveInput": false,

  // 控制文件被其他某些进程删除或重命名时是否应该自动关闭显示文件的编辑器。禁用此项会保持编辑器作为此类事件的脏文件打开。请注意，从应用程序内部进行删除操作会始终关闭编辑器，并且脏文件始终不会关闭以保存数据。
  "workbench.editor.closeOnFileDelete": true,

  // 控制是否将打开的编辑器显示为预览。预览编辑器将会重用至其被保留(例如，通过双击或编辑)，且其字体样式将为斜体。
  "workbench.editor.enablePreview": true,

  // 控制 Quick Open 中打开的编辑器是否显示为预览。预览编辑器可以重新使用，直到将其保留(例如，通过双击或编辑)。
  "workbench.editor.enablePreviewFromQuickOpen": true,

  // 控制编辑器标签的格式。修改这项设置会让文件的路径更容易理解：
  // - short: "parent"
  // - medium: "workspace/src/parent"
  // - long: "/home/user/workspace/src/parent"
  // - default: 当与另一选项卡标题相同时为 ".../parent"。选项卡被禁用时则为相对工作区路径
  "workbench.editor.labelFormat": "default",

  // 控制打开编辑器的位置。选择“左侧”或“右侧”以在当前活动位置的左侧或右侧打开编辑器。选择“第一个”或“最后一个”以从当前活动位置独立打开编辑器。
  "workbench.editor.openPositioning": "right",

  // 控制打开时编辑器是否显示在任何可见组中。如果禁用，编辑器会优先在当前活动编辑器组中打开。如果启用，会显示已打开的编辑器而不是在当前活动编辑器组中再次打开。请注意，有些情况下会忽略此设置，例如强制编辑器在特定组中或在当前活动组的边侧打开时。
  "workbench.editor.revealIfOpen": false,

  // 控制打开的编辑器是否随图标一起显示。这还需启用图标主题。
  "workbench.editor.showIcons": true,

  // 控制打开的编辑器是否显示在选项卡中。
  "workbench.editor.showTabs": true,

  // 控制编辑器的选项卡关闭按钮的位置，或当设置为 "off" 时禁用关闭它们。
  "workbench.editor.tabCloseButton": "right",

  // 控制编辑器选项卡的大小。若设置为 "fit"，选项卡将总是足够大，能够完全显示编辑器标签。若设置为 "shrink"，将在不能一次全部显示所有选项卡时，允许选项卡缩小。
  "workbench.editor.tabSizing": "fit",

  // 指定在工作台中使用的图标主题，或指定 "null" 以不显示任何文件图标。
  "workbench.iconTheme": "vs-seti",

  // 在通过鼠标多选树和列表条目时使用的修改键 (例如资资源管理器、打开的编辑器和源代码管理视图)。"ctrlCmd" 会映射为 "Ctrl" (Windows 和 Linux) 或 "Command" (macOS)。“打开到侧边”功能所需的鼠标动作 (若可用) 将会相应调整，不与多选修改键冲突。
  "workbench.list.multiSelectModifier": "ctrlCmd",

  // 控制如何在受支持的树和列表中使用鼠标来打开项目。设置为 "singleClick" 可单击打开项目，"doubleClick" 仅可双击打开项目。对于树中含子节点的节点，此设置将控制使用单击还是双击来展开他们。注意，某些不适用此项的树或列表可能会忽略此设置。
  "workbench.list.openMode": "singleClick",

  // 控制此面板的默认位置。可显示在工作台的底部或右侧。
  "workbench.panel.defaultLocation": "bottom",

  // 控制 Quick Open 是否应在失去焦点时自动关闭。
  "workbench.quickOpen.closeOnFocusLost": true,

  // 控制是否在设置中启用自然语言搜索模式。
  "workbench.settings.enableNaturalLanguageSearch": true,

  // 控制打开设置时是否打开显示所有默认设置的编辑器。
  "workbench.settings.openDefaultSettings": true,

  // 控制边栏的位置。它可显示在工作台的左侧或右侧。
  "workbench.sideBar.location": "left",

  // 在未能恢复上一会话信息的情况下，控制启动时显示的编辑器。选择 "none" 表示启动时不打开编辑器，"welcomePage" 表示打开欢迎页面(默认)，"newUntitledFile" 表示打开新的无标题文档(仅打开一个空工作区)。
  "workbench.startupEditor": "welcomePage",

  // 控制是否显示工作台底部状态栏中的 Twitter 反馈 (笑脸图标)。
  "workbench.statusBar.feedback.visible": true,

  // 控制工作台底部状态栏的可见性。
  "workbench.statusBar.visible": true,

  // 启用后，当没有打开编辑器时将显示水印提示。
  "workbench.tips.enabled": true

}
,
{


  // 控制关闭最后一个编辑器是否关闭整个窗口。此设置仅适用于不显示文件夹的窗口。
  "window.closeWhenEmpty": false,

  // 如果启用，则可使用 Alt 快捷键打开主菜单。禁用助记键允许将这些 Alt 快捷键绑定到编辑器命令。
  "window.enableMenuBarMnemonics": true,

  // 控制菜单栏的可见性。“切换”设置表示隐藏菜单栏，按一次 Alt 键则将显示此菜单栏。默认情况下，除非窗口为全屏，否则菜单栏可见。
  "window.menuBarVisibility": "default",

  // 控制在已有窗口时新打开窗口的尺寸。默认情况下，新窗口将以小尺寸在屏幕的中央打开。当设置为“inherit”时，新窗口将继承上一活动窗口的尺寸，设置为“maximized”时窗口将被最大化，设置为“fullscreen”时则变为全屏。请注意，此设置对第一个打开的窗口无效。第一个窗口总是会恢复关闭前的大小和位置。
  "window.newWindowDimensions": "default",

  // 控制是否应在新窗口中打开文件。
  // - default: 文件将在该文件的文件夹打开的窗口中打开，或在上一个活动窗口中打开，除非该文件通过平台或从查找程序(仅限 macOS)打开
  // - on: 文件将在新窗口中打开
  // - off: 文件将在该文件的文件夹打开的窗口中打开，或在上一个活动窗口中打开
  // 注意，可能仍会存在忽略此设置的情况(例如当使用 -new-window 或 -reuse-window 命令行选项时)。
  "window.openFilesInNewWindow": "off",

  // 控制文件夹应在新窗口中打开还是替换上一活动窗口。
  // - default: 文件夹将在新窗口中打开，除非文件是从应用程序内选取的(例如通过“文件”菜单)
  // - on: 文件夹将在新窗口中打开
  // - off: 文件夹将替换上一活动窗口
  // 注意，可能仍会存在忽略此设置的情况(例如当使用 -new-window 或 -reuse-window 命令行选项时)。
  "window.openFoldersInNewWindow": "default",

  // 如果窗口已退出全屏模式，控制其是否应还原为全屏模式。
  "window.restoreFullscreen": false,

  // 控制重启后重新打开窗口的方式。选择 "none" 则永远在启动时打开一个空工作区，"one" 则重新打开最后使用的窗口，"folders" 则重新打开所有含有文件夹的窗口，"all" 则重新打开上次会话的所有窗口。
  "window.restoreWindows": "one",

  // 根据活动编辑器控制窗口标题。变量基于上下文进行替换:
  // ${activeEditorShort}: 文件名 (如 myFile.txt)
  // ${activeEditorMedium}: 相对于工作区文件夹的文件路径 (如 myFolder/myFile.txt)
  // ${activeEditorLong}: 文件的完整路径 (如 /Users/Development/myProject/myFolder/myFile.txt)
  // ${folderName}: 文件所在工作区文件夹名称 (如 myFolder)
  // ${folderPath}: 文件所在工作区文件夹路径 (如 /Users/Development/myFolder)
  // ${rootName}: 工作区名称 (如 myFolder 或 myWorkspace)
  // ${rootPath}: 工作区路径 (如 /Users/Development/myWorkspace)
  // ${appName}: 如 VS Code
  // ${dirty}: 活动编辑器有更新时显示的更新指示器
  // ${separator}: 仅在被有值变量包围时显示的分隔符 (" - ")
  "window.title": "${dirty}${activeEditorShort}${separator}${rootName}${separator}${appName}",

  // 调整窗口的缩放级别。原始大小是 0，每次递增(例如 1)或递减(例如 -1)表示放大或缩小 20%。也可以输入小数以便以更精细的粒度调整缩放级别。
  "window.zoomLevel": 0

}
,
{


  // 控制打开 Zen Mode 是否也会将工作台置于全屏模式。
  "zenMode.fullScreen": true,

  // 控制打开 Zen 模式是否也会隐藏工作台左侧的活动栏。
  "zenMode.hideActivityBar": true,

  // 控制打开 Zen 模式是否也会隐藏工作台底部的状态栏。
  "zenMode.hideStatusBar": true,

  // 控制打开 Zen 模式是否也会隐藏工作台选项卡。
  "zenMode.hideTabs": true,

  // 控制如果某窗口已退出 zen 模式，是否应还原到 zen 模式。
  "zenMode.restore": false

}
,
{


  // 配置语言的文件关联(如: "*.extension": "html")。这些关联的优先级高于已安装语言的默认关联。
  "files.associations": {},

  // 如果启用，会在打开文件时尝试猜测字符集编码。也可以根据语言配置此设置。
  "files.autoGuessEncoding": false,

  // 控制已更新文件的自动保存。接受的值:“off”、"afterDelay”、“onFocusChange”(编辑器失去焦点)、“onWindowChange”(窗口失去焦点)。如果设置为“afterDelay”，则可在 "files.autoSaveDelay" 中配置延迟。
  "files.autoSave": "off",

  // 控制在多少毫秒后自动保存更改过的文件。仅在“files.autoSave”设置为“afterDelay”时适用。
  "files.autoSaveDelay": 1000,

  // 分配给新文件的默认语言模式。
  "files.defaultLanguage": "",

  // 读取和编写文件时使用的默认字符集编码。也可以根据语言配置此设置。
  "files.encoding": "utf8",

  // 默认行尾字符。使用 \n 表示 LF，\r\n 表示 CRLF。
  "files.eol": "\r\n",

  // 配置 glob 模式以在搜索中排除文件和文件夹。例如，文件资源管理器根据此设置决定文件或文件夹的显示和隐藏。
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true
  },

  // 控制是否在会话间记住未保存的文件，以允许在退出编辑器时跳过保存提示。
  "files.hotExit": "onExit",

  // 启用后，保存文件时在文件末尾插入一个最终新行。
  "files.insertFinalNewline": false,

  // 启用后，保存文件时将删除在最终新行后的所有新行。
  "files.trimFinalNewlines": false,

  // 启用后，将在保存文件时剪裁尾随空格。
  "files.trimTrailingWhitespace": false,

  // 使用新的试验文件观察程序。
  "files.useExperimentalFileWatcher": false,

  // 配置文件路径的 glob 模式以从文件监视排除。模式必须在绝对路径上匹配(例如 ** 前缀或完整路径需正确匹配)。更改此设置需要重启。如果在启动时遇到 Code 消耗大量 CPU 时间，则可以排除大型文件夹以减少初始加载。
  "files.watcherExclude": {
    "**/.git/objects/**": true,
    "**/.git/subtree-cache/**": true,
    "**/node_modules/*/**": true
  }

}
,
{


  // 控制资源管理器是否应在打开文件时自动显示并选择它们。
  "explorer.autoReveal": true,

  // 控制资源管理器是否应在删除文件到回收站时进行确认。
  "explorer.confirmDelete": true,

  // 控制在资源管理器内拖放移动文件或文件夹时是否进行确认。
  "explorer.confirmDragAndDrop": true,

  // 控制文件修饰是否用徽章。
  "explorer.decorations.badges": true,

  // 控制文件修饰是否用颜色。
  "explorer.decorations.colors": true,

  // 控制资源管理器是否应该允许通过拖放移动文件和文件夹。
  "explorer.enableDragAndDrop": true,

  // 在“打开的编辑器”窗格中显示的编辑器数量。
  "explorer.openEditors.visible": 9,

  // 控制资源管理器文件和文件夹的排列顺序。除了默认排列顺序，你也可以设置为 "mixed" (文件和文件夹一起排序)、"type" (按文件类型排)、"modified" (按最后修改日期排)或是 "filesFirst" (将文件排在文件夹前)。
  "explorer.sortOrder": "default"

}
,
{


  // 配置 glob 模式以在搜索中排除文件和文件夹。从 files.exclude 设置中继承所有 glob 模式。
  "search.exclude": {
    "**/node_modules": true,
    "**/bower_components": true
  },

  // 控制是否在搜索中跟踪符号链接。
  "search.followSymlinks": true,

  // 配置为在 Quick Open 文件结果中包括全局符号搜索的结果。
  "search.quickOpen.includeSymbols": false,

  // 若搜索词全为小写，则不区分大小写进行搜索，否则区分大小写进行搜索
  "search.smartCase": false,

  // 控制搜索文件时是否使用 .gitignore 和 .ignore 文件。
  "search.useIgnoreFiles": true,

  // 控制是否在文本和文件搜索中使用 ripgrep
  "search.useRipgrep": true

}
,
{


  // 要使用的代理设置。如果尚未设置，则将从 http_proxy 和 https_proxy 环境变量获取
  "http.proxy": "",

  // 要作为每个网络请求的 "Proxy-Authorization" 标头发送的值。
  "http.proxyAuthorization": null,

  // 是否应根据提供的 CA 列表验证代理服务器证书。
  "http.proxyStrictSSL": true

}
,
{


  // 配置是否从更新通道接收自动更新。更改后需要重启。
  "update.channel": "default",

  // 启用 Windows 后台更新。
  "update.enableWindowsBackgroundUpdates": false

}
,
{


  // 启用/禁用 HTML 标记的自动关闭。
  "html.autoClosingTags": true,

  // 以逗号分隔的标记列表，不应在其中重新设置内容的格式。"null" 默认为 "pre" 标记。
  "html.format.contentUnformatted": "pre,code,textarea",

  // 启用/禁用默认 HTML 格式化程序
  "html.format.enable": true,

  // 以新行结束。
  "html.format.endWithNewline": false,

  // 标记列表，以逗号分隔，其前应有额外新行。"null" 默认为“标头、正文、/html”。
  "html.format.extraLiners": "head, body, /html",

  // 格式和缩进 {{#foo}} 和 {{/foo}}。
  "html.format.indentHandlebars": false,

  // 缩进 <head> 和 <body> 部分。
  "html.format.indentInnerHtml": false,

  // 要保留在一个区块中的换行符的最大数量。对于无限制使用 "null"。
  "html.format.maxPreserveNewLines": null,

  // 是否要保留元素前面的现有换行符。仅适用于元素前，不适用于标记内或文本。
  "html.format.preserveNewLines": true,

  // 以逗号分隔的标记列表不应重设格式。"null" 默认为所有列于 https://www.w3.org/TR/html5/dom.html#phrasing-content 的标记。
  "html.format.unformatted": "wbr",

  // 对属性进行换行。
  "html.format.wrapAttributes": "auto",

  // 每行最大字符数(0 = 禁用)。
  "html.format.wrapLineLength": 120,

  // 配置内置 HTML 语言支持是否建议 Angular V1 标记和属性。
  "html.suggest.angular1": true,

  // 配置内置 HTML 语言支持是否建议 HTML5 标记、属性和值。
  "html.suggest.html5": true,

  // 配置内置 HTML 语言支持是否建议 Ionic 标记、属性和值。
  "html.suggest.ionic": true,

  // 跟踪 VS Code 与 HTML 语言服务器之间的通信。
  "html.trace.server": "off",

  // 配置内置的 HTML 语言支持是否对嵌入的脚本进行验证。
  "html.validate.scripts": true,

  // 配置内置的 HTML 语言支持是否对嵌入的样式进行验证。
  "html.validate.styles": true

}
,
{


  // 启用/禁用默认 JSON 格式化程序(需要重启)
  "json.format.enable": true,

  // 将当前项目中的 JSON 文件与架构关联起来
  "json.schemas": [],

  // 跟踪 VS Code 与 JSON 语言服务器之间的通信。
  "json.trace.server": "off"

}
,
{


  // 设置换行符如何在 markdown 预览中呈现。将其设置为 "true" 会为每一个新行创建一个 <br>。
  "markdown.preview.breaks": false,

  // 在 Markdown 预览中双击切换到编辑器。
  "markdown.preview.doubleClickToSwitchToEditor": true,

  // 控制 Markdown 预览中使用的字体系列。
  "markdown.preview.fontFamily": "-apple-system, BlinkMacSystemFont, 'Segoe WPC', 'Segoe UI', 'HelveticaNeue-Light', 'Ubuntu', 'Droid Sans', sans-serif",

  // 控制 Markdown 预览中使用的字号(以像素为单位)。
  "markdown.preview.fontSize": 14,

  // 控制 Markdown 预览中使用的行高。此数值与字号相关。
  "markdown.preview.lineHeight": 1.6,

  // 在 Markdown 预览中启用或禁用将类似 URL 的文本转换为链接。
  "markdown.preview.linkify": true,

  // 在 Markdown 预览中标记当前的编辑器选定内容。
  "markdown.preview.markEditorSelection": true,

  // 当 Markdown 预览滚动时，更新编辑器的视图。
  "markdown.preview.scrollEditorWithPreview": true,

  // 滚动 Markdown 预览以显示编辑器中当前所选的行。
  "markdown.preview.scrollPreviewWithEditorSelection": true,

  // 设置如何在 Markdown 预览中呈现 YAML 扉页。“隐藏”会删除扉页。否则，扉页则被视为 Markdown 内容。
  "markdown.previewFrontMatter": "hide",

  // 要在 Markdown 预览中使用的 CSS 样式表的 URL 或本地路径列表。相对路径被解释为相对于资源管理器中打开的文件夹。如果没有任何打开的文件夹，则会被解释为相对于 Markdown 文件的位置。所有的 "\" 需写为 "\\"。
  "markdown.styles": [],

  // 对 Markdown 扩展启用调试日志记录。
  "markdown.trace": "off"

}
,
{


  // 如果已启用内置 PHP 语言建议，则进行配置。此支持建议 PHP 全局变量和变量。
  "php.suggest.basic": true,

  // 启用/禁用内置的 PHP 验证。
  "php.validate.enable": true,

  // 指向 PHP 可执行文件。
  "php.validate.executablePath": null,

  // 决定 linter 是在保存时还是输入时运行。
  "php.validate.run": "onSave"

}
,
{


  // 启用/禁用 JavaScript 格式化程序。
  "javascript.format.enable": true,

  // 定义逗号分隔符后面的空格处理。
  "javascript.format.insertSpaceAfterCommaDelimiter": true,

  // 定义构造器关键字后的空格处理。要求 TypeScript >= 2.3.0。
  "javascript.format.insertSpaceAfterConstructor": false,

  // 定义匿名函数的函数关键字后面的空格处理。
  "javascript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": true,

  // 定义控制流语句中关键字后面的空格处理。
  "javascript.format.insertSpaceAfterKeywordsInControlFlowStatements": true,

  // 定义 JSX 表达式左括号后面和右括号前面的空格处理。要求 TypeScript >= 2.0.6。
  "javascript.format.insertSpaceAfterOpeningAndBeforeClosingJsxExpressionBraces": false,

  // 定义非空括号的左括号后面和右括号前面的空格处理。要求 TypeScript >= 2.3.0。
  "javascript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBraces": true,

  // 定义非空方括号的左括号后面和右括号前面的空格处理。
  "javascript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBrackets": false,

  // 定义非空圆括号的左括号后面和右括号前面的空格处理。
  "javascript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyParenthesis": false,

  // 定义模板字符串的左括号后面和右括号前面的空格处理。要求 TypeScript >= 2.0.6。
  "javascript.format.insertSpaceAfterOpeningAndBeforeClosingTemplateStringBraces": false,

  // 在 For 语句中，定义分号后面的空格处理。
  "javascript.format.insertSpaceAfterSemicolonInForStatements": true,

  // 定义二进制运算符后面的空格处理
  "javascript.format.insertSpaceBeforeAndAfterBinaryOperators": true,

  // 在函数参数括号前定义空格处理。需要 TypeScript >= 2.1.5。
  "javascript.format.insertSpaceBeforeFunctionParenthesis": false,

  // 定义控制块的左括号是否放置在新的一行。
  "javascript.format.placeOpenBraceOnNewLineForControlBlocks": false,

  // 定义函数的左大括号是否放置在新的一行。
  "javascript.format.placeOpenBraceOnNewLineForFunctions": false,

  // 启用/禁用 JavaScript 文件的语义检查。现有的 jsconfig.json 或
  //  tsconfig.json 文件会覆盖此设置。要求 TypeScript >=2.3.1。
  "javascript.implicitProjectConfig.checkJs": false,

  // 对不属于任何工程的 JavaScript 文件启用或禁用 "experimentalDecorators" 设置。现有的 jsconfig.json 或
  //  tsconfig.json 文件会覆盖此设置。要求 TypeScript >=2.3.1。
  "javascript.implicitProjectConfig.experimentalDecorators": false,

  // 启用/禁用在 JavaScript 建议列表中包含文件中的唯一名称。
  "javascript.nameSuggestions": true,

  // 启用/禁用在 JavaScript 文件中引用 CodeLens。
  "javascript.referencesCodeLens.enabled": false,

  // 启用/禁用 JavaScript 验证。
  "javascript.validate.enable": true,

  // 启用/禁用自动 JSDoc 注释
  "jsDocCompletion.enabled": true,

  // 启用或禁用自动导入建议。要求 TypeScript >= 2.6.1
  "typescript.autoImportSuggestions.enabled": true,

  // 检查是否安装了 NPM 以自动获取类型。
  "typescript.check.npmIsInstalled": true,

  // 禁用自动获取类型。需要 TypeScript >= 2.0.6。
  "typescript.disableAutomaticTypeAcquisition": false,

  // 启用/禁用默认 TypeScript 格式化程序。
  "typescript.format.enable": true,

  // 定义逗号分隔符后面的空格处理。
  "typescript.format.insertSpaceAfterCommaDelimiter": true,

  // 定义构造器关键字后的空格处理。要求 TypeScript >= 2.3.0。
  "typescript.format.insertSpaceAfterConstructor": false,

  // 定义匿名函数的函数关键字后面的空格处理。
  "typescript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": true,

  // 定义控制流语句中关键字后面的空格处理。
  "typescript.format.insertSpaceAfterKeywordsInControlFlowStatements": true,

  // 定义 JSX 表达式左括号后面和右括号前面的空格处理。要求 TypeScript >= 2.0.6。
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingJsxExpressionBraces": false,

  // 定义非空括号的左括号后面和右括号前面的空格处理。要求 TypeScript >= 2.3.0。
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBraces": true,

  // 定义非空方括号的左括号后面和右括号前面的空格处理。
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBrackets": false,

  // 定义非空圆括号的左括号后面和右括号前面的空格处理。
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyParenthesis": false,

  // 定义模板字符串的左括号后面和右括号前面的空格处理。要求 TypeScript >= 2.0.6。
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingTemplateStringBraces": false,

  // 在 For 语句中，定义分号后面的空格处理。
  "typescript.format.insertSpaceAfterSemicolonInForStatements": true,

  // 定义 TypeScript 中类型断言后的空格处理。要求 TypeScript >= 2.4。
  "typescript.format.insertSpaceAfterTypeAssertion": false,

  // 定义二进制运算符后面的空格处理
  "typescript.format.insertSpaceBeforeAndAfterBinaryOperators": true,

  // 在函数参数括号前定义空格处理。需要 TypeScript >= 2.1.5。
  "typescript.format.insertSpaceBeforeFunctionParenthesis": false,

  // 定义控制块的左括号是否放置在新的一行。
  "typescript.format.placeOpenBraceOnNewLineForControlBlocks": false,

  // 定义函数的左大括号是否放置在新的一行。
  "typescript.format.placeOpenBraceOnNewLineForFunctions": false,

  // 启用/禁用实现 CodeLens。要求 TypeScript >= 2.2.0。
  "typescript.implementationsCodeLens.enabled": false,

  // 设置报告 TypeScript 错误时使用的区域设置。要求 TypeScript >= 2.6.0。默认 ("null") 将使用 VS Code 的区域设置。
  "typescript.locale": null,

  // 指定用于自动获取类型的 NPM 可执行文件的路径。要求 TypeScript >= 2.3.4。
  "typescript.npm": null,

  // 当输入导入路径时启用或禁用快速建议。
  "typescript.quickSuggestionsForPaths": true,

  // 启用/禁用在 TypeScript 文件中引用 CodeLens。要求 TypeScript >= 2.0.6。
  "typescript.referencesCodeLens.enabled": false,

  // 将风格检查问题报告为警告
  "typescript.reportStyleChecksAsWarnings": true,

  // 控制 tsc 任务的自动检测。"off" 关闭此功能。"build" 仅创建单次运行编译任务。"watch" 仅创建编译及监视任务。"on" 创建构建及监视任务。默认值为 "on"。
  "typescript.tsc.autoDetect": "on",

  // 指定包含要使用的 tsserver 和 lib*.d.ts 文件的文件夹路径。
  "typescript.tsdk": null,

  // 将 TS 服务器的日志保存到一个文件。此日志可用于诊断 TS 服务器问题。日志可能包含你的项目中的文件路径、源代码和其他可能敏感的信息。
  "typescript.tsserver.log": "off",

  // 对发送到 TS 服务器的消息启用跟踪。此跟踪信息可用于诊断 TS 服务器问题。 跟踪信息可能包含你的项目中的文件路径、源代码和其他可能敏感的信息。
  "typescript.tsserver.trace": "off",

  // 完成函数的参数签名。
  "typescript.useCodeSnippetsOnMethodSuggest": false,

  // 启用/禁用 TypeScript 验证。
  "typescript.validate.enable": true

}
,
{


  // 允许在任何文件中设置断点
  "debug.allowBreakpointsEverywhere": false,

  // 控制是否应该隐藏浮点调试操作栏
  "debug.hideActionBar": false,

  // 调试时，在编辑器中显示变量值内联
  "debug.inlineValues": false,

  // 内部调试控制台的控制行为。
  "debug.internalConsoleOptions": "openOnFirstSessionStart",

  // 控制是否在调试会话开始时打开调试侧边栏面板。
  "debug.openDebug": "openOnFirstSessionStart",

  // 调试会话结束时自动打开资源管理器视图
  "debug.openExplorerOnEnd": false,

  // 控制何时显示调试状态栏
  "debug.showInStatusBar": "onFirstSessionStart",

  // 全局的调试启动配置。应用作跨工作区共享的 "launch.json" 的替代。
  "launch": {}

}
,
{


  // 参数数量无效
  "css.lint.argumentsInColorFunction": "error",

  // 使用边距或边框时，不要使用宽度或高度
  "css.lint.boxModel": "ignore",

  // 使用供应商特定前缀时，确保同时包括所有其他供应商特定属性
  "css.lint.compatibleVendorPrefixes": "ignore",

  // 不要使用重复的样式定义
  "css.lint.duplicateProperties": "ignore",

  // 不要使用空规则集
  "css.lint.emptyRules": "warning",

  // 避免使用“float”。浮动会带来脆弱的 CSS，如果布局的某一方面更改，将很容易破坏 CSS。
  "css.lint.float": "ignore",

  // @font-face 规则必须定义 "src" 和 "font-family" 属性
  "css.lint.fontFaceProperties": "warning",

  // 十六进制颜色必须由三个或六个十六进制数字组成
  "css.lint.hexColorLength": "error",

  // 选择器不应包含 ID，因为这些规则与 HTML 的耦合过于紧密。
  "css.lint.idSelector": "ignore",

  // 仅当支持 IE7 及更低版本时，才需要 IE hack
  "css.lint.ieHack": "ignore",

  // 避免使用 !important。它表明整个 CSS 的特异性已经失去控制且需要重构。
  "css.lint.important": "ignore",

  // Import 语句不会并行加载
  "css.lint.importStatement": "ignore",

  // 因显示而忽略属性。例如，使用 "display: inline"时，宽度、高度、上边距、下边距和 float 属性将不起作用
  "css.lint.propertyIgnoredDueToDisplay": "warning",

  // 通配选择符 (*) 运行效率低
  "css.lint.universalSelector": "ignore",

  // 未知的属性。
  "css.lint.unknownProperties": "warning",

  // 未知的供应商特定属性。
  "css.lint.unknownVendorSpecificProperties": "ignore",

  // 使用供应商特定前缀时，还应包括标准属性
  "css.lint.vendorPrefix": "warning",

  // 零不需要单位
  "css.lint.zeroUnits": "ignore",

  // 跟踪 VS Code 与 CSS 语言服务器之间的通信。
  "css.trace.server": "off",

  // 启用或禁用所有验证
  "css.validate": true

}
,
{


  // 参数数量无效
  "less.lint.argumentsInColorFunction": "error",

  // 使用边距或边框时，不要使用宽度或高度
  "less.lint.boxModel": "ignore",

  // 使用供应商特定前缀时，确保同时包括所有其他供应商特定属性
  "less.lint.compatibleVendorPrefixes": "ignore",

  // 不要使用重复的样式定义
  "less.lint.duplicateProperties": "ignore",

  // 不要使用空规则集
  "less.lint.emptyRules": "warning",

  // 避免使用“float”。浮动会带来脆弱的 CSS，如果布局的某一方面更改，将很容易破坏 CSS。
  "less.lint.float": "ignore",

  // @font-face 规则必须定义 "src" 和 "font-family" 属性
  "less.lint.fontFaceProperties": "warning",

  // 十六进制颜色必须由三个或六个十六进制数字组成
  "less.lint.hexColorLength": "error",

  // 选择器不应包含 ID，因为这些规则与 HTML 的耦合过于紧密。
  "less.lint.idSelector": "ignore",

  // 仅当支持 IE7 及更低版本时，才需要 IE hack
  "less.lint.ieHack": "ignore",

  // 避免使用 !important。它表明整个 CSS 的特异性已经失去控制且需要重构。
  "less.lint.important": "ignore",

  // Import 语句不会并行加载
  "less.lint.importStatement": "ignore",

  // 因显示而忽略属性。例如，使用 "display: inline"时，宽度、高度、上边距、下边距和 float 属性将不起作用
  "less.lint.propertyIgnoredDueToDisplay": "warning",

  // 已知通配选择符 (*) 慢
  "less.lint.universalSelector": "ignore",

  // 未知的属性。
  "less.lint.unknownProperties": "warning",

  // 未知的供应商特定属性。
  "less.lint.unknownVendorSpecificProperties": "ignore",

  // 使用供应商特定前缀时，还应包括标准属性
  "less.lint.vendorPrefix": "warning",

  // 零不需要单位
  "less.lint.zeroUnits": "ignore",

  // 启用或禁用所有验证
  "less.validate": true

}
,
{


  // 参数数量无效
  "scss.lint.argumentsInColorFunction": "error",

  // 使用边距或边框时，不要使用宽度或高度
  "scss.lint.boxModel": "ignore",

  // 使用供应商特定前缀时，确保同时包括所有其他供应商特定属性
  "scss.lint.compatibleVendorPrefixes": "ignore",

  // 不要使用重复的样式定义
  "scss.lint.duplicateProperties": "ignore",

  // 不要使用空规则集
  "scss.lint.emptyRules": "warning",

  // 避免使用“float”。浮动会带来脆弱的 CSS，如果布局的某一方面更改，将很容易破坏 CSS。
  "scss.lint.float": "ignore",

  // @font-face 规则必须定义 "src" 和 "font-family" 属性
  "scss.lint.fontFaceProperties": "warning",

  // 十六进制颜色必须由三个或六个十六进制数字组成
  "scss.lint.hexColorLength": "error",

  // 选择器不应包含 ID，因为这些规则与 HTML 的耦合过于紧密。
  "scss.lint.idSelector": "ignore",

  // 仅当支持 IE7 及更低版本时，才需要 IE hack
  "scss.lint.ieHack": "ignore",

  // 避免使用 !important。它表明整个 CSS 的特异性已经失去控制且需要重构。
  "scss.lint.important": "ignore",

  // Import 语句不会并行加载
  "scss.lint.importStatement": "ignore",

  // 因显示而忽略属性。例如，使用 "display: inline"时，宽度、高度、上边距、下边距和 float 属性将不起作用
  "scss.lint.propertyIgnoredDueToDisplay": "warning",

  // 已知通配选择符 (*) 慢
  "scss.lint.universalSelector": "ignore",

  // 未知的属性。
  "scss.lint.unknownProperties": "warning",

  // 未知的供应商特定属性。
  "scss.lint.unknownVendorSpecificProperties": "ignore",

  // 使用供应商特定前缀时，还应包括标准属性
  "scss.lint.vendorPrefix": "warning",

  // 零不需要单位
  "scss.lint.zeroUnits": "ignore",

  // 启用或禁用所有验证
  "scss.validate": true

}
,
{


  // 自动更新扩展
  "extensions.autoUpdate": true,

  // 如果设置为 "true"，将不再显示扩展建议的通知。
  "extensions.ignoreRecommendations": false

}
,
{


  // 自定义要启动的终端类型。
  "terminal.explorerKind": "integrated",

  // 自定义要在 Linux 上运行的终端。
  "terminal.external.linuxExec": "xterm",

  // 自定义要在 OS X 上运行的终端应用程序。
  "terminal.external.osxExec": "Terminal.app",

  // 自定义要在 Windows 上运行的终端。
  "terminal.external.windowsExec": "C:\\WINDOWS\\System32\\cmd.exe"

}
,
{


  // 一组命令 ID，其键绑定不发送到 shell 而始终由 Code 处理。这使得通常由 shell 使用的键绑定的使用效果与未将终端设为焦点时相同，例如按 Ctrl+P 启动 Quick Open。
  "terminal.integrated.commandsToSkipShell": [
    "editor.action.toggleTabFocusMode",
    "workbench.action.debug.continue",
    "workbench.action.debug.pause",
    "workbench.action.debug.restart",
    "workbench.action.debug.run",
    "workbench.action.debug.start",
    "workbench.action.debug.stepInto",
    "workbench.action.debug.stepOut",
    "workbench.action.debug.stepOver",
    "workbench.action.debug.stop",
    "workbench.action.focusActiveEditorGroup",
    "workbench.action.focusFirstEditorGroup",
    "workbench.action.focusSecondEditorGroup",
    "workbench.action.focusThirdEditorGroup",
    "workbench.action.navigateDown",
    "workbench.action.navigateLeft",
    "workbench.action.navigateRight",
    "workbench.action.navigateUp",
    "workbench.action.openNextRecentlyUsedEditorInGroup",
    "workbench.action.openPreviousRecentlyUsedEditorInGroup",
    "workbench.action.quickOpen",
    "workbench.action.quickOpenPreviousEditor",
    "workbench.action.quickOpenView",
    "workbench.action.showCommands",
    "workbench.action.tasks.build",
    "workbench.action.tasks.restartTask",
    "workbench.action.tasks.runTask",
    "workbench.action.tasks.showLog",
    "workbench.action.tasks.showTasks",
    "workbench.action.tasks.terminate",
    "workbench.action.tasks.test",
    "workbench.action.terminal.clear",
    "workbench.action.terminal.copySelection",
    "workbench.action.terminal.deleteWordLeft",
    "workbench.action.terminal.deleteWordRight",
    "workbench.action.terminal.findWidget.history.showNext",
    "workbench.action.terminal.findWidget.history.showPrevious",
    "workbench.action.terminal.focus",
    "workbench.action.terminal.focusAtIndex1",
    "workbench.action.terminal.focusAtIndex2",
    "workbench.action.terminal.focusAtIndex3",
    "workbench.action.terminal.focusAtIndex4",
    "workbench.action.terminal.focusAtIndex5",
    "workbench.action.terminal.focusAtIndex6",
    "workbench.action.terminal.focusAtIndex7",
    "workbench.action.terminal.focusAtIndex8",
    "workbench.action.terminal.focusAtIndex9",
    "workbench.action.terminal.focusFindWidget",
    "workbench.action.terminal.focusNext",
    "workbench.action.terminal.focusPrevious",
    "workbench.action.terminal.hideFindWidget",
    "workbench.action.terminal.kill",
    "workbench.action.terminal.new",
    "workbench.action.terminal.newInActiveWorkspace",
    "workbench.action.terminal.paste",
    "workbench.action.terminal.runActiveFile",
    "workbench.action.terminal.runSelectedText",
    "workbench.action.terminal.scrollDown",
    "workbench.action.terminal.scrollDownPage",
    "workbench.action.terminal.scrollToBottom",
    "workbench.action.terminal.scrollToTop",
    "workbench.action.terminal.scrollUp",
    "workbench.action.terminal.scrollUpPage",
    "workbench.action.terminal.selectAll",
    "workbench.action.terminal.toggleTerminal",
    "workbench.action.togglePanel"
  ],

  // 在存在活动终端会话的情况下，退出时是否要确认。
  "terminal.integrated.confirmOnExit": false,

  // 设置后，终端中选中的文字将被复制到剪贴板。
  "terminal.integrated.copyOnSelection": false,

  // 控制终端光标是否闪烁。
  "terminal.integrated.cursorBlinking": false,

  // 控制终端游标的样式。
  "terminal.integrated.cursorStyle": "block",

  // 将在其中启动终端的一个显式起始路径，它用作 shell 进程的当前工作目录(cwd)。当根目录为不方便的 cwd 时，此路径在工作区设置中可能十分有用。
  "terminal.integrated.cwd": "",

  // 是否启用终端响铃。
  "terminal.integrated.enableBell": false,

  // 要添加到 VS Code 进程中的带有环境变量的对象，其会被 Linux 终端使用。
  "terminal.integrated.env.linux": {},

  // 要添加到 VS Code 进程中的带有环境变量的对象，其会被 OS X 终端使用。
  "terminal.integrated.env.osx": {},

  // 要添加到 VS Code 进程中的带有环境变量的对象，其会被 Windows 终端使用。
  "terminal.integrated.env.windows": {},

  // 控制终端的字体系列，这在编辑器中是默认的。fontFamily 的值。
  "terminal.integrated.fontFamily": "",

  // 控制终端的字号(以像素为单位)。
  "terminal.integrated.fontSize": 14,

  // 终端中非粗体字使用的字重。
  "terminal.integrated.fontWeight": "normal",

  // 终端中粗体字使用的字重。
  "terminal.integrated.fontWeightBold": "bold",

  // 控制终端的行高，此数字乘上终端字号得到实际行高(以像素为单位)。
  "terminal.integrated.lineHeight": 1,

  // 在终端中，使用 Option 键作为 Meta 键。(macOS)
  "terminal.integrated.macOptionIsMeta": false,

  // 设置后，在终端内右键单击时，这将阻止显示上下文菜单，相反，它将在有选项时进行复制，并且在没有选项时进行粘贴。
  "terminal.integrated.rightClickCopyPaste": true,

  // 控制终端保持在缓冲区的最大行数。
  "terminal.integrated.scrollback": 1000,

  // 控制是否在终端启动时设置区域设置变量，在 OS X 上默认设置为 true，在其他平台上为 false。
  "terminal.integrated.setLocaleVariables": false,

  // 终端在 Linux 上使用的 shell 的路径。
  "terminal.integrated.shell.linux": "sh",

  // 终端在 OS X 上使用的 shell 的路径。
  "terminal.integrated.shell.osx": "sh",

  // 终端在 Windows 使用的 shell 路径。使用随 Windows 一起提供的 shell (cmd、PowerShell 或 Bash on Ubuntu) 时。
  "terminal.integrated.shell.windows": "C:\\WINDOWS\\System32\\WindowsPowerShell\\v1.0\\powershell.exe",

  // 在 Linux 终端上时要使用的命令行参数。
  "terminal.integrated.shellArgs.linux": [],

  // 在 OS X 终端上时要使用的命令行参数。
  "terminal.integrated.shellArgs.osx": [
    "-l"
  ],

  // 在 Windows 终端上时使用的命令行参数。
  "terminal.integrated.shellArgs.windows": [],

  // 当退出代码非零时，显示“终端进程以某退出代码终止”的警告。
  "terminal.integrated.showExitAlert": true

}
,
{


  // 控制问题预览是否应在打开文件时自动显示它们。
  "problems.autoReveal": true,

  // 显示关于文件与文件夹的错误与警告。
  "problems.decorations.enabled": true

}
,
{


  // 启用要发送给 Microsoft 的故障报表。
  // 此选项需重启才可生效。
  "telemetry.enableCrashReporter": true,

  // 启用要发送给 Microsoft 的使用情况数据和错误。
  "telemetry.enableTelemetry": true

}
,
{


  // 针对 [git-commit] 语言，配置替代编辑器设置。
  "[git-commit]":  {
    "editor.rulers": [
        72
    ]
  },

  // 针对 [go] 语言，配置替代编辑器设置。
  "[go]":  {
    "editor.insertSpaces": false
  },

  // 针对 [json] 语言，配置替代编辑器设置。
  "[json]":  {
    "editor.quickSuggestions": {
        "strings": true
    }
  },

  // 针对 [makefile] 语言，配置替代编辑器设置。
  "[makefile]":  {
    "editor.insertSpaces": false
  },

  // 针对 [markdown] 语言，配置替代编辑器设置。
  "[markdown]":  {
    "editor.wordWrap": "on",
    "editor.quickSuggestions": false
  },

  // 针对 [yaml] 语言，配置替代编辑器设置。
  "[yaml]":  {
    "editor.insertSpaces": true,
    "editor.tabSize": 2,
    "editor.quickSuggestions": {
        "other": true,
        "comments": false,
        "strings": true
    },
    "editor.autoIndent": false
  }

}
,
{


  // 控制自动检测 Jake 任务是否打开。默认开启。
  "jake.autoDetect": "on"

}
,
{


  // 控制自动检测 Gulp 任务是否打开。默认开启。
  "gulp.autoDetect": "on"

}
,
{


  // 是否启用自动拉取
  "git.autofetch": false,

  // 是否启用自动刷新
  "git.autorefresh": true,

  // 是否自动检测存储库
  "git.autoRepositoryDetection": true,

  // 控制运行“签出到...”功能时列出的分支类型。"all" 显示所有 refs，"local" 只显示本地分支，"tags" 只显示标签，"remote" 只显示远程分支。
  "git.checkoutType": "all",

  // 同步 GIT 存储库前请先进行确认
  "git.confirmSync": true,

  // 控制 Git 徽章计数器。“all”计算所有更改。“tracked”只计算跟踪的更改。“off”关闭此功能。
  "git.countBadge": "all",

  // 控制 Git 是否向资源管理器和“打开的编辑器”视图添加颜色和小标。
  "git.decorations.enabled": true,

  // 克隆 Git 存储库的默认位置
  "git.defaultCloneDirectory": null,

  // 控制是否自动检测 Git 子模块。
  "git.detectSubmodules": true,

  // 启用使用 GPG 签名的提交
  "git.enableCommitSigning": false,

  // 是否启用 Git
  "git.enabled": true,

  // 在没有暂存的更改时提交所有更改。
  "git.enableSmartCommit": false,

  // 忽略旧版 Git 警告
  "git.ignoreLegacyWarning": false,

  // 忽略“存储库中存在大量更改”的警告
  "git.ignoreLimitWarning": false,

  // 忽略“缺失 Git”警告
  "git.ignoreMissingGitWarning": false,

  // 控制何时显示输入验证输入计数。
  "git.inputValidation": "warn",

  // Git 可执行文件路径
  "git.path": null,

  // 控制 Git 是否在提交之前检查未保存的文件。
  "git.promptToSaveFilesBeforeCommit": false,

  // 控制是否在 Git 更改视图中显示内联“打开文件”操作。
  "git.showInlineOpenFileAction": true

}
,
{


  // Custom tags for the parser to use
  "yaml.customTags": [],

  // Enable/disable default YAML formatter (requires restart)
  "yaml.format.enable": false,

  // Associate schemas to Yaml files in the current workspace
  "yaml.schemas": {},

  // Traces the communication between VSCode and the languageServerExample service.
  "yaml.trace.server": "off",

  // Enable/disable validation feature
  "yaml.validate": true

}
,
{


  // Automatically add brackets for functions.
  "python.autoComplete.addBrackets": false,

  // List of paths to libraries and the like that need to be imported by auto complete engine. E.g. when using Google App SDK, the paths are not in system path, hence need to be added into this list.
  "python.autoComplete.extraPaths": [],

  // Comma delimited list of modules preloaded to speed up Auto Complete (e.g. add Numpy, Pandas, etc, items slow to load when autocompleting).
  "python.autoComplete.preloadModules": [],

  // Controls appearance of methods with double underscores in the completion list.
  "python.autoComplete.showAdvancedMembers": false,

  // Whether to check if Python is installed (also warn when using the macOS-installed Python).
  "python.disableInstallationCheck": false,

  // Do not display a prompt to install these features
  "python.disablePromptForFeatures": [],

  // Absolute path to a file containing environment variable definitions.
  "python.envFile": "${workspaceFolder}/.env",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.formatting.autopep8Args": [],

  // Path to autopep8, you can use a custom version of autopep8 by modifying this setting to include the full path.
  "python.formatting.autopep8Path": "autopep8",

  // Provider for formatting. Possible options include 'autopep8' and 'yapf'.
  "python.formatting.provider": "autopep8",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.formatting.yapfArgs": [],

  // Path to yapf, you can use a custom version of yapf by modifying this setting to include the full path.
  "python.formatting.yapfPath": "yapf",

  // Whether to install Python modules globally when not using an environment.
  "python.globalModuleInstallation": false,

  // Memory limit for the Jedi completion engine in megabytes. Zero (default) means 1024 MB. -1 means unlimited (disable memory limit check)
  "python.jediMemoryLimit": 0,

  // Path to directory containing the Jedi library (this path will contain the 'Jedi' sub directory).
  "python.jediPath": "",

  // Whether to lint Python files.
  "python.linting.enabled": true,

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.flake8Args": [],

  // Severity of Flake8 message type 'E'.
  "python.linting.flake8CategorySeverity.E": "Error",

  // Severity of Flake8 message type 'F'.
  "python.linting.flake8CategorySeverity.F": "Error",

  // Severity of Flake8 message type 'W'.
  "python.linting.flake8CategorySeverity.W": "Warning",

  // Whether to lint Python files using flake8
  "python.linting.flake8Enabled": false,

  // Path to flake8, you can use a custom version of flake8 by modifying this setting to include the full path.
  "python.linting.flake8Path": "flake8",

  // Patterns used to exclude files or folders from being linted.
  "python.linting.ignorePatterns": [
    ".vscode/*.py",
    "**/site-packages/**/*.py"
  ],

  // Whether to lint Python files when saved.
  "python.linting.lintOnSave": true,

  // Controls the maximum number of problems produced by the server.
  "python.linting.maxNumberOfProblems": 100,

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.mypyArgs": [
    "--ignore-missing-imports",
    "--follow-imports=silent"
  ],

  // Severity of Mypy message type 'Error'.
  "python.linting.mypyCategorySeverity.error": "Error",

  // Severity of Mypy message type 'Note'.
  "python.linting.mypyCategorySeverity.note": "Information",

  // Whether to lint Python files using mypy.
  "python.linting.mypyEnabled": false,

  // Path to mypy, you can use a custom version of mypy by modifying this setting to include the full path.
  "python.linting.mypyPath": "mypy",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.pep8Args": [],

  // Severity of Pep8 message type 'E'.
  "python.linting.pep8CategorySeverity.E": "Error",

  // Severity of Pep8 message type 'W'.
  "python.linting.pep8CategorySeverity.W": "Warning",

  // Whether to lint Python files using pep8
  "python.linting.pep8Enabled": false,

  // Path to pep8, you can use a custom version of pep8 by modifying this setting to include the full path.
  "python.linting.pep8Path": "pep8",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.prospectorArgs": [],

  // Whether to lint Python files using prospector.
  "python.linting.prospectorEnabled": false,

  // Path to Prospector, you can use a custom version of prospector by modifying this setting to include the full path.
  "python.linting.prospectorPath": "prospector",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.pydocstyleArgs": [],

  // Whether to lint Python files using pydocstyle
  "python.linting.pydocstyleEnabled": false,

  // Path to pydocstyle, you can use a custom version of pydocstyle by modifying this setting to include the full path.
  "python.linting.pydocstylePath": "pydocstyle",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.pylamaArgs": [],

  // Whether to lint Python files using pylama.
  "python.linting.pylamaEnabled": false,

  // Path to pylama, you can use a custom version of pylama by modifying this setting to include the full path.
  "python.linting.pylamaPath": "pylama",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.linting.pylintArgs": [],

  // Severity of Pylint message type 'Convention/C'.
  "python.linting.pylintCategorySeverity.convention": "Information",

  // Severity of Pylint message type 'Error/E'.
  "python.linting.pylintCategorySeverity.error": "Error",

  // Severity of Pylint message type 'Fatal/F'.
  "python.linting.pylintCategorySeverity.fatal": "Error",

  // Severity of Pylint message type 'Refactor/R'.
  "python.linting.pylintCategorySeverity.refactor": "Hint",

  // Severity of Pylint message type 'Warning/W'.
  "python.linting.pylintCategorySeverity.warning": "Warning",

  // Whether to lint Python files using pylint.
  "python.linting.pylintEnabled": true,

  // Path to Pylint, you can use a custom version of pylint by modifying this setting to include the full path.
  "python.linting.pylintPath": "pylint",

  // Whether to run Pylint with minimal set of rules.
  "python.linting.pylintUseMinimalCheckers": true,

  // Path to Python, you can use a custom version of Python by modifying this setting to include the full path.
  "python.pythonPath": "python",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.sortImports.args": [],

  // Path to isort script, default using inner version
  "python.sortImports.path": "",

  // Activate Python Environment in Terminal created using the Extension.
  "python.terminal.activateEnvironment": true,

  // When executing a file in the terminal, whether to use execute in the file's directory, instead of the current open folder.
  "python.terminal.executeInFileDir": false,

  // Python launch arguments to use when executing a file in the terminal.
  "python.terminal.launchArgs": [],

  // Optional working directory for unit tests.
  "python.unitTest.cwd": null,

  // IP Address of the of the local unit test server (default is localhost or use 127.0.0.1).
  "python.unitTest.debugHost": "localhost",

  // Port number used for debugging of unittests.
  "python.unitTest.debugPort": 3000,

  // Arguments passed in. Each argument is a separate item in the array.
  "python.unitTest.nosetestArgs": [],

  // Path to nosetests, you can use a custom version of nosetests by modifying this setting to include the full path.
  "python.unitTest.nosetestPath": "nosetests",

  // Whether to enable or disable unit testing using nosetests.
  "python.unitTest.nosetestsEnabled": false,

  // Where to prompt to configure a test framework if potential tests directories are discovered.
  "python.unitTest.promptToConfigure": true,

  // Arguments passed in. Each argument is a separate item in the array.
  "python.unitTest.pyTestArgs": [],

  // Whether to enable or disable unit testing using pytest.
  "python.unitTest.pyTestEnabled": false,

  // Path to pytest (pytest), you can use a custom version of pytest by modifying this setting to include the full path.
  "python.unitTest.pyTestPath": "pytest",

  // Arguments passed in. Each argument is a separate item in the array.
  "python.unitTest.unittestArgs": [
    "-v",
    "-s",
    ".",
    "-p",
    "*test*.py"
  ],

  // Whether to enable or disable unit testing using unittest.
  "python.unitTest.unittestEnabled": false,

  // Use the experimental debugger when debugging unit tests.
  "python.unitTest.useExperimentalDebugger": false,

  // Folders in your home directory to look into for virtual environments.
  "python.venvFolders": [
    "envs",
    ".pyenv",
    ".direnv"
  ],

  // Path to folder with a list of Virtual Environments (e.g. ~/.pyenv, ~/Envs, ~/.virtualenvs).
  "python.venvPath": "",

  // Fully qualilified path to the ctags executable (else leave as ctags, assuming it is in current path).
  "python.workspaceSymbols.ctagsPath": "ctags",

  // Set to 'false' to disable Workspace Symbol provider using ctags.
  "python.workspaceSymbols.enabled": true,

  // Pattern used to exclude files and folders from ctags See http://ctags.sourceforge.net/ctags.html.
  "python.workspaceSymbols.exclusionPatterns": [
    "**/site-packages/**"
  ],

  // Whether to re-build the tags file on when changes made to python files are saved.
  "python.workspaceSymbols.rebuildOnFileSave": true,

  // Whether to re-build the tags file on start (defaults to true).
  "python.workspaceSymbols.rebuildOnStart": true,

  // Fully qualified path to tag file (exuberant ctag file), used to provide workspace symbols.
  "python.workspaceSymbols.tagFilePath": "${workspaceFolder}/.vscode/tags"

}
,
{


  // Math formula delimiters.
  "mdmath.delimiters": "dollars"

}
,
{


  // markdownlint config object
  "markdownlint.config": {
    "MD013": false
  },

  // Array of paths for custom rules to include when linting
  "markdownlint.customRules": [],

  // Array of file names and glob expressions to ignore when linting
  "markdownlint.ignore": [],

  // Run the linter on save (onSave) or on type (onType)
  "markdownlint.run": "onType"

}
,
{


  // 不应展开 Emmet 缩写的语言数组。
  "emmet.excludeLanguages": [
    "markdown"
  ],

  // 包含 Emmet 配置文件与代码片段的文件夹路径。
  "emmet.extensionsPath": null,

  // 在默认不支持 Emmet 的语言中启用 Emmet 缩写功能。在此添加该语言与支持 Emmet 的语言之间的映射。
  // 示例: {"vue-html": "html", "javascript": "javascriptreact"}
  "emmet.includeLanguages": {},

  // 用于修改 Emmet 某些操作和解析程序的行为的首选项。
  "emmet.preferences": {},

  // 显示可能的 Emmet 缩写作为建议。在样式表中或当 emmet.showExpandedAbbreviation 设置为 "never" 时不适用。
  "emmet.showAbbreviationSuggestions": true,

  // 在建议中显示展开的 Emmet 缩写。
  // 选择 "inMarkupAndStylesheetFilesOnly" 选项将仅应用于 html、haml、jade、slim、xml、xsl、css、scss、sass、less 和 stylus 文件。
  // 选择 "always" 选项将应用于所有适用文件不限于标记或 CSS 的所有部分。
  "emmet.showExpandedAbbreviation": "always",

  // 若为 "true"，Emmet 建议将显示为代码片段。你可以在 editor.snippetSuggestions 设置中排列顺序。
  "emmet.showSuggestionsAsSnippets": false,

  // 为指定的语法定义配置文件或使用带有特定规则的配置文件。
  "emmet.syntaxProfiles": {},

  // 启用后，按下 TAB 键，将展开 Emmet 缩写。
  "emmet.triggerExpansionOnTab": false,

  // 用于 Emmet 代码片段的变量
  "emmet.variables": {}

}
,
{


  // 控制自动检测 Grunt 任务是否打开。默认开启。
  "grunt.autoDetect": "on"

}
,
{


  // 控制自动检测 npm 脚本是否打开。默认开启。
  "npm.autoDetect": "on",

  // 用于运行脚本的程序包管理器。
  "npm.packageManager": "npm",

  // 使用 "--silent" 选项运行 npm 命令。
  "npm.runSilent": false

}
,
{


  // 启用/禁用编辑器内合并冲突区域的 CodeLens
  "merge-conflict.codeLens.enabled": true,

  // 启用/禁用编辑器内的合并冲突修饰器
  "merge-conflict.decorators.enabled": true

}
,
{


  // 控制搜索文件时是否使用 .gitignore 和 .ignore 文件。
  "search.useIgnoreFiles": true,

  // 针对 [git-commit] 语言，配置替代编辑器设置。
  "[git-commit]": {
    "editor.rulers": [
      72
    ]
  },

  // 是否启用自动拉取
  "git.autofetch": false,

  // 是否启用自动刷新
  "git.autorefresh": true,

  // 是否自动检测存储库
  "git.autoRepositoryDetection": true,

  // 控制运行“签出到...”功能时列出的分支类型。"all" 显示所有 refs，"local" 只显示本地分支，"tags" 只显示标签，"remote" 只显示远程分支。
  "git.checkoutType": "all",

  // 同步 GIT 存储库前请先进行确认
  "git.confirmSync": true,

  // 控制 Git 徽章计数器。“all”计算所有更改。“tracked”只计算跟踪的更改。“off”关闭此功能。
  "git.countBadge": "all",

  // 控制 Git 是否向资源管理器和“打开的编辑器”视图添加颜色和小标。
  "git.decorations.enabled": true,

  // 克隆 Git 存储库的默认位置
  "git.defaultCloneDirectory": null,

  // 控制是否自动检测 Git 子模块。
  "git.detectSubmodules": true,

  // 启用使用 GPG 签名的提交
  "git.enableCommitSigning": false,

  // 是否启用 Git
  "git.enabled": true,

  // 在没有暂存的更改时提交所有更改。
  "git.enableSmartCommit": false,

  // 忽略旧版 Git 警告
  "git.ignoreLegacyWarning": false,

  // 忽略“存储库中存在大量更改”的警告
  "git.ignoreLimitWarning": false,

  // 忽略“缺失 Git”警告
  "git.ignoreMissingGitWarning": false,

  // 控制何时显示输入验证输入计数。
  "git.inputValidation": "warn",

  // Git 可执行文件路径
  "git.path": null,

  // 控制 Git 是否在提交之前检查未保存的文件。
  "git.promptToSaveFilesBeforeCommit": false,

  // 控制是否在 Git 更改视图中显示内联“打开文件”操作。
  "git.showInlineOpenFileAction": true
