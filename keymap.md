# Раскладка

## Editor - Редактор

Копирование и вставка:

map <C-v> :action $Paste<CR>:action EditorEscape<CR>
ap <C-c> :action $Copy<CR>:action EditorEscape<CR>
ap <C-x> :action $Cut<CR>
ap y :action $Copy<CR>v:action EditorEscape<CR>
ap p :action $Paste<CR>v:action EditorEscape<CR>
