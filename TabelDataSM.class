/*
 * To change this template, choose Tools | Templates
 * and open the template in the editor.
 */
package tabel;
import java.util.ArrayList;
import java.util.List;
import javax.swing.table.AbstractTableModel;
/**
 *
 * @author Ita Masita
 */
 
        public class TabelDataSM extends AbstractTableModel {
 
        private List<DataSM> list = new ArrayList<>();
 
        @Override
        public int getRowCount() {
            return list.size();
        }
 
        @Override
        public int getColumnCount() {
            return 8;
        }
 
        @Override
        public Object getValueAt(int rowIndex, int columnIndex) {
            switch (columnIndex) {
                case 0:
                    return list.get(rowIndex).getTgl();
                case 1:
                    return list.get(rowIndex).getNo();
                case 2:
                    return list.get(rowIndex).getNo_Surat();
                case 3:
                    return list.get(rowIndex).getTgl_Surat();
                case 4:
                    return list.get(rowIndex).getDari();
                case 5:
                    return list.get(rowIndex).getIsi();
                case 6:
                    return list.get(rowIndex).getLampiran();
                case 7:
                    return list.get(rowIndex).getKet();
                default:
                    return null;
            }
        }
 
        @Override
        public String getColumnName(int kolom) {
            switch (kolom) {
                case 0:
                    return "Tanggal";
                case 1:
                    return "No.";
                case 2:
                    return "No. Surat";
                case 3:
                    return "Tanggal Surat";
                case 4:
                    return "Pengirim";
                case 5:
                    return "Perihal";
                case 6:
                    return "Lampiran";
                case 7:
                    return "Keterangan";
                default:
                    return null;
            }
        }
 
        public void add(DataSM sm) {
            list.add(sm);
            fireTableRowsInserted(getRowCount(), getColumnCount());
        }
 
        public void delete(int i, int baris) {
            list.remove(i);
            fireTableRowsDeleted(i, baris);
        }
 
        public DataSM get(int baris) {
            return (DataSM) list.get(baris);
        }
    }