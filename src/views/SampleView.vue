<template>
  <div class="theme-green">
    <div class="qs-app-wrapper" style="min-height:45vh !important;">
      <div class="qs-component">
        <div class="qs-text">
          <label class="qs-text__label active-label">사원명</label>
          <div class="qs-text__input">
            <input type="text" placeholder="Please input" class="el-input__inner" />
          </div>
        </div>

        <div class="qs-list">
          <el-table
            :data="tableData"
            header-row-class-name="qs-list__header-row"
            header-cell-class-name="qs-list__header-cell"
            max-height="250"
            style="width: 100%">
            <el-table-column
              prop="date"
              label="Date">
            </el-table-column>
            <el-table-column label="Delivery Info">
              <el-table-column
                prop="name"
                label="Name">
              </el-table-column>
              <el-table-column label="Address Info">
                <el-table-column
                  prop="state"
                  label="State">
                </el-table-column>
                <el-table-column
                  prop="city"
                  label="City">
                </el-table-column>
                <el-table-column
                  prop="address"
                  label="Address">
                </el-table-column>
                <el-table-column
                  prop="zip"
                  label="Zip">
                </el-table-column>
              </el-table-column>
            </el-table-column>
          </el-table>
        </div>
      </div>
    </div>
  </div>
  <div class="theme-kakao">
    <div class="qs-app-wrapper" style="min-height:45vh !important">
      <div class="qs-component">
        <div class="qs-text">
          <label class="qs-text__label active-label">사원명</label>
          <div class="qs-text__input active-label-form el-input el-input--medium">
            <input type="text" placeholder="Please input" class="el-input__inner" />
          </div>
        </div>

        <div class="qs-list">
          <el-table
            :data="tableData"
            header-row-class-name="qs-list__header-row"
            header-cell-class-name="qs-list__header-cell"
            max-height="250"
            style="width: 100%">
            <el-table-column
              prop="date"
              label="Date">
            </el-table-column>
            <el-table-column label="Delivery Info">
              <el-table-column
                prop="name"
                label="Name">
              </el-table-column>
              <el-table-column label="Address Info">
                <el-table-column
                  prop="state"
                  label="State">
                </el-table-column>
                <el-table-column
                  prop="city"
                  label="City">
                </el-table-column>
                <el-table-column
                  prop="address"
                  label="Address">
                </el-table-column>
                <el-table-column
                  prop="zip"
                  label="Zip">
                </el-table-column>
              </el-table-column>
            </el-table-column>
          </el-table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
      return {
        tableData: [{
          date: '2016-05-03',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }, {
          date: '2016-05-02',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }, {
          date: '2016-05-04',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }, {
          date: '2016-05-01',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }, {
          date: '2016-05-08',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }, {
          date: '2016-05-06',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }, {
          date: '2016-05-07',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036'
        }]
      }
    }
};
</script>
