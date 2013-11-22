# 演示文档

---



<form class="form-inline sandbox-form" id="sandbox">
        <div class="well">
          Type:<br>

          <label for="markup-text" class="inline radio">
            <input name="markup" id="markup-text" value="input" type="radio" checked="">
            Text input
            <script type="text/html" class="html">
              <input type="text">
            </script>
            <script type="text/plain" class="selector">
              input
            </script>
          </label>
          <label for="markup-component" class="inline radio">
            <input name="markup" id="markup-component" value="component" type="radio">
            Component
            <script type="text/html" class="html">
              <div class="input-append date">
                <input type="text" class="span2"><span class="add-on"><i class="icon-th"></i></span>
              </div>
            </script>
            <script type="text/plain" class="selector">
              .input-append.date
            </script>
          </label>
          <label for="markup-inline" class="inline radio">
            <input name="markup" id="markup-inline" value="embedded" type="radio">
            Embedded / inline
            <script type="text/html" class="html">
              <div></div>
            </script>
            <script type="text/plain" class="selector">
              div
            </script>
          </label>
          <label for="markup-range" class="inline radio">
            <input name="markup" id="markup-range" value="range" type="radio">
            Range
            <script type="text/html" class="html">
              <div class="input-daterange" id="datepicker">
                  <input type="text" class="input-small" name="start" />
                  <span class="add-on">to</span>
                  <input type="text" class="input-small" name="end" />
              </div>
            </script>
            <script type="text/plain" class="selector">
              .input-daterange
            </script>
          </label>

          <br><br>

          Options:<br>

          <label for="format">Format
            <input class="span2" id="format" name="format" type="text" placeholder="mm/dd/yyyy"></label>
          <label for="weekStart">Week start
            <input class="span1" id="weekStart" name="weekStart" type="text" placeholder="0"></label>
          <label for="startDate">Start date
            <input class="span2" id="startDate" name="startDate" type="text" placeholder="-Infinity"></label>
          <label for="endDate">End date
            <input class="span2" id="endDate" name="endDate" type="text" placeholder="+Infinity"></label>
          <label for="startView">Start view
            <select class="span2" id="startView" name="startView">
              <option value="0">0 / month</option>
              <option value="1">1 / year</option>
              <option value="2">2 / decade</option>
            </select>
          </label>
          <label for="minViewMode">Min view mode
            <select class="span2" id="minViewMode" name="minViewMode">
              <option value="0">0 / days</option>
              <option value="1">1 / months</option>
              <option value="2">2 / years</option>
            </select>
          </label>
          <label for="todayBtn" class="inline checkbox">Today button
            <select class="span2" id="todayBtn" name="todayBtn">
              <option value="false">disabled</option>
              <option value="true">enabled (unlinked)</option>
              <option value="linked">linked</option>
            </select>
          </label>
          <label for="language">Language
            <select class="span1" id="language" name="language">
              <option value="en">en</option>
            <option value="ar">ar</option><option value="bg">bg</option><option value="ca">ca</option><option value="cs">cs</option><option value="da">da</option><option value="de">de</option><option value="el">el</option><option value="es">es</option><option value="et">et</option><option value="fi">fi</option><option value="fr">fr</option><option value="he">he</option><option value="hr">hr</option><option value="hu">hu</option><option value="id">id</option><option value="is">is</option><option value="it">it</option><option value="ja">ja</option><option value="ka">ka</option><option value="kr">kr</option><option value="lt">lt</option><option value="lv">lv</option><option value="mk">mk</option><option value="ms">ms</option><option value="nb">nb</option><option value="nl">nl</option><option value="no">no</option><option value="pl">pl</option><option value="pt-BR">pt-BR</option><option value="pt">pt</option><option value="ro">ro</option><option value="rs">rs</option><option value="rs-latin">rs-latin</option><option value="ru">ru</option><option value="sk">sk</option><option value="sl">sl</option><option value="sq">sq</option><option value="sv">sv</option><option value="sw">sw</option><option value="th">th</option><option value="tr">tr</option><option value="uk">uk</option><option value="zh-CN">zh-CN</option><option value="zh-TW">zh-TW</option></select>
            <script>
             /* $(function(){
                for (var lang in $.fn.datepicker.dates) {
                  if (!$('#language option[value='+lang+']').length)
                    $('<option value="'+lang+'">'+lang+'</option>').appendTo('#language')
                }
              });*/
            </script>
          </label>
          <label for="orientation">Orientation
            <select class="span2" id="orientation" name="orientation">
              <option value="auto">auto</option>
              <option value="top auto">top auto</option>
              <option value="bottom auto">bottom auto</option>
              <option value="auto left">auto left</option>
              <option value="top left">top left</option>
              <option value="bottom left">bottom left</option>
              <option value="auto right">auto right</option>
              <option value="top right">top right</option>
              <option value="bottom right">bottom right</option>
            </select>
          </label>

          <br>

          <span>Days of week disabled:
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="0"> 0</label>
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="1"> 1</label>
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="2"> 2</label>
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="3"> 3</label>
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="4"> 4</label>
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="5"> 5</label>
            <label class="checkbox"><input type="checkbox" name="daysOfWeekDisabled" value="6"> 6</label>
          </span>

          <br>

          <label for="calendarWeeks" class="inline checkbox">
            <input id="calendarWeeks" name="calendarWeeks" type="checkbox">
            Calendar weeks
          </label>
          <label for="autoclose" class="inline checkbox">
            <input id="autoclose" name="autoclose" type="checkbox">
            Autoclose
          </label>
          <label for="todayHighlight" class="inline checkbox">
            <input id="todayHighlight" name="todayHighlight" type="checkbox">
            Today highlight
          </label>
          <label for="keyboardNavigation" class="inline checkbox">
            <input id="keyboardNavigation" name="keyboardNavigation" type="checkbox" checked="">
            Keyboard navigation
          </label>
          <label for="forceParse" class="inline checkbox">
            <input id="forceParse" name="forceParse" type="checkbox" checked="">
            Force parse
          </label>
          <label for="beforeShowDay" class="inline checkbox">
            <input id="beforeShowDay" name="beforeShowDay" type="checkbox">
            Before-show-day callback
          </label>

          <br><br>

          <button class="btn btn-danger" type="reset">Reset to defaults</button>
        </div>
      </form>

<style>
    .datepicker table tr:nth-child(2n) {background-color:#fff;}
    .datepicker table tr {border-top:none;}
</style>


````javascript
seajs.use('datepicker.css');
seajs.use('datepicker', function($){
   $('#datepicker').datepicker();
});
````

<input id="datepicker" type="text">

