# TpPackage








package IpPckage;
public class IpPackage{
        private int o1;
        private int o2;
        private int o3;
        private int o4;

        private IpPackage (int var0, int var1, int var2, int var3){
                this.o1=var0;
                this.o2=var1;
                this.o3=var2;
                this.o4=var3;
                }
                public static IpPackage getinstance(int var0, int var1, int var2, int var3){
                        try{
                                if (var0<0||var0>255||var1<0||var1>255||var2<0||var2>255||var3<0||var3>255){
                                        throw new Exception();
                                }
                        } catch(Exception var5){
                                System.out.print("Valeur impossible /n");
                        }

                        System.out.print("o1="+var0);
                        System.out.print("o2="+var1);
                        System.out.print("o3="+var2);
                        System.out.print("o4="+var3);
                        return new IpPackage(var0, var1, var2, var3);

        }
}
