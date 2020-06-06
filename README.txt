Autores:
Sara Rodríguez Velásquez
Alejandro Díaz Cano
Juan Sebastián Vega Correa

Solucionamos el punto 1 "Triangulos y texturas"

Modificando

El metodo computeNormal y computeUV de la siguiente manera:
 
	public Vector4 computeNormal(Point p) {
        	Vector4 vA= new Vector4(p.x-v1.x,p.y-v2.x,p.z-v2.x);
        	Vector4 vB= new Vector4(v2.x-v1.x,v2.y-v2.x,v2.z-v2.x);
        	Vector4 lanormal = normal.crossProduct(vA,vB);
        	return normal;
    	}


	public UVCoordinates computeUV(Point p) {
        	double u,v;
        	u= Math.atan(p.y/p.x);
        	v = p.z:
        	return new UVCoordinates(u, v);

	}



¿como ejecutar el programa?
*El proyecto se abre en netbeans, se ejecuta la clase llamada llamada "main.java" que encontramos en el paquete View.


